# InferenceAgent
Agent that performs inference in first order logic-implements backward chaining algorithm in Python

Input should be in the following format:
<#queries>
<queries>
<#rules>
<rules>

eg:
1
X(C)
4
A(x,y) ^ B(x,y) => X(z)
E(X) => A(x,x)
E(X)
B(Y,Y)

Each rule is in one of these two formats:
1- p1 ∧ p2 ∧ ... ∧ pn => q
2- facts: which are atomic sentences. Such as p or ~p

Output will be either "TRUE" or "FALSE" for each query.
