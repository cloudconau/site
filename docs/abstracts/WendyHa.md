# Wendy Ha - SEEK
## Anatomy of a Kubernetes Release Cycle: A Practical Guide for End Users
### Abstract
Upstream Kubernetes is the open-source core of Kubernetes, maintained by the Cloud Native Computing Foundation (CNCF). It contains the pure source code and documentation for orchestrating containers, without vendor-specific extensions, and is fully open for anyone to inspect, contribute to, or redistribute.

Because of its open-source nature, anyone can ""fork"" the core Kubernetes codebase to create their own version. Over the past 11 years, many organizations, including vendors and cloud providers, have created “fork” versions of Kubernetes, modify upstream code to meet their own needs, then package and offer it as proprietary Kubernetes distributions.

Most end users are more familiar with these vendor-provided Kubernetes offerings and rely on them. However, upstream Kubernetes has always remained as the source of truth, it's the heart where decisions are made, features are proposed and developed, and the broader community collaborates to improve the ecosystem.

As a member of the Kubernetes Release Team, I'll walk you through the lifecycle of a Kubernetes release process, including how new features are proposed via KEPs (Kubernetes Enhancement Proposals), tracked, and progress through Alpha, Beta, and GA stages? What does the typical 4-month release cycle looks like, from Planning, Development, Code Freeze, and Release? Key milestones and deadlines that end users and contributors should be aware of?

This talk will use the newest Kubernetes v1.34, scheduled just a week before the CloudCon Sydney 2025, as a real-world example. It is ideal for anyone curious about how a large open-source project like Kubernetes operates behind the scenes, especially for those who want to better understand when and how new features get landed, and eventually you can contribute to make it better.

### Speaker Bio

[Wendy](https://www.linkedin.com/in/wendyha-sut/){target=_blank} is a Software Engineer with passion across Platform Engineering, Site Reliability and Observability. In her role, she helps teams build systems that are not just scalable, but reliable and resilient. Wendy is also an open source contributor and has contributed to various aspects of Kubernetes, including SIG Release (serving on the Release Team since v1.31), SIG Cluster Lifecycle and SIG Etcd. She's currently taken on leadership roles as the Release Signal Lead for Kubernetes v1.33 and Release Lead Shadow for v1.34, where she focuses on improving release processes and mentoring new contributors into the open source space.

Wendy is a proud advocate for Women in Tech, the Deaf and Hard of Hearing community, and Women-led Entrepreneurship. She's passionate about making complex technologies easy to understand and make the Cloud Native space more inclusive and accessible.

When she's not coding or contributing to the community, you'll find her enjoying a cup of coffee or exploring the Dandenong trails in Melbourne. She's also deeply committed to mental health advocacy and breaking the stigma around mental wellbeing in tech.