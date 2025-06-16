# COMO FUNCIONA

Explicación simple de como funciona DEB


```mermaid
flowchart TD
    A[DEB] --> |Run Script| B[build]
    B --> Z[Git repositories:<br/>- github.com/user01/repo1<br/>- github.com/user02/repo2<br/>- github.com/user03/repo3]
    Z --> C{git clone \$repo}

    C --> |user01| D[repo1]
    C --> |user02| E[repo2]
    C --> |user03| F[repo3]

    D --> |Run Script| D2[build]
    E --> |Run Script| E2[build]
    F --> |Run Script| F2[build]

    D2 --> G1[package1.deb]
    E2 --> G2[package2.deb]
    F2 --> G3[package3.deb]

    G1 --> H[reprepro]
    G2 --> H
    G3 --> H

    H --> I[nlbol.github.io/deb/plurios]    