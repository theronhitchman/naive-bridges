# Loop Lemma

Let K be a knot, and let [n ,k, n+1, k'] be an element of its PD code, where
k' = k+1 or k' = k-1. The two incoming strands are then labelled with either
n and k (in the first case) or n and k'=k-1 (in the second case).

*Lemma*: The two incoming strands must have opposite parity.

Proof: Let P be the double point in the projection of K which corresponds to
our chosen piece of the PD code.

Of the two incoming strands, one comes _first_ and the other _second_
in standard ordering of the natural numbers. Let the smaller one be m and the
larger one be m'.

By way of contradiction, assume that the numbers m and m' have the same parity.

        m' = m + 2M, for some M>0

Consider the portion of the knot projection which starts at and ends at our
specified crossing, leaving at index m+1 and returning at index m'. This is a
closed loop, L, based at the double point at our crossing. We have chosen L to
be formed by the portion of the knot from the first outgoing strand from P to
the second incoming strand to P.

So the rest of the knot L' = K-L must form a loop from P which crosses the loop
L an even number of times away from P.

But our indices along are

    m'+1 (going out from P), m'+2, ..., m'-1, m' = m+2M (return to P).

But that means there are an _odd_ number of such crossings, which is a
contradiction.

Hence the two incoming strands must have opposite parities.

QED.
