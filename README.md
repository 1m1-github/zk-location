# zk-location
zero knowledge prove device location within a circle

a signed app knows gets the device location

zkp with

public inputs: 
1) coordinates on a sphere (circle center =: C)
2) radius (r)

private inputs: own coordinates on a sphere (location =: l)

circom circuit estimates spherical distance between the C and l =: d(C,l)

zkp <=> d(C,l) <= r

use case:
social apps to prove location without compromising privacy

vs https://www.stratumn.com/en/blog/zero-knowledge-proof-of-location, we zkp that location is within an arbitrary circle, not amongst "a list of authorized areas"
