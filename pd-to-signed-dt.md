# How to Turn a PD Code into a Signed DT Code

## Note on PD code

Suppose K is an oriented knot diagram with n crossings.

A PD code is a list of n different ordered 4-tuples, one for each crossing.

At a crossing, we have a 4-tuple of the form [m,k,m+1,k'] where k'= k+1 or k-1.
The numbers label arcs of the diagram between crossings, in order along the
direction of travel.

    * the 4-tuple [m,k,m+1,k+1] represents a left-handed crossing
      where the strand m-(m+1) goes under the strand k-(k+1).
    * the 4-tuple [m,k,m+1,k-1] represents a right-handed crossing
      where the strand m-(m+1) goes under the strand k-(k-1).

Note that we always read the 4-tuple code of a single crossing by starting at
the arc with lowest index and then working around counter-clockwise.

## Note on signed DT code

Normal DT code assigns two numbers to each crossing, one even and one odd.

1. But this loses the information about which over and which is under.
  (This is properly implied for alternating knots, but requires extra info for
  knots which are not alternating.) To fix that, we add a 'u' mark to the
  number representing the strand which goes under.

2. Also, it loses the information about handedness of the crossing. to rectify
  this, we add a + for right-handed crossings and a - for left-handed crossings.

As such, the signed DT code will be a list of symbols that look like this:

```
     N                uN
    uK      or         K
    +/-               +/-
```

## How to transform a PD code into a DT code.

Each 4-tuple in the PD code corresponds to a crossing, so it will give us one
piece of the DT code.
