---
title: "Create diagrams as code with Mermaid"
date: 2022-09-26T12:46:08-05:00
author: Daniel Velázquez
draft: true
tags: ["mermaid", "hugo"]
---

### Mermiad

{{< mermaid align="left" theme="neutral" >}}
sequenceDiagram
title Token Based

Client ->> Server: POST /login <br> {email,password}
Note right of Server: Create JWT for User <br> w/ secret

Server -->> Client: Send JWT
Note left of Client: Store Token <br> as localStorage

Client ->> Server: Send Request <br> with JWT <br> In Header (Authorization:BearerToken )
Note right of Server: Verify JWT Signature
Server -->> Client: Send Response

{{< /mermaid >}}
