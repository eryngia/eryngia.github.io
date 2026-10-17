---
title: "Software Engineer Intern"
collection: experience
company: "ING Group"
location: "Brussels, Belgium"
date: "2023-06-01"
date_range: "June 2023 – July 2023"
permalink: /experience/software-engineer-intern/
summary:
  - Developed a RESTful microservice in Scala using http4s for testing a global messaging system.
  - Designed and built utilities for Kafka stream testing in a distributed environment.
  - Collaborated with engineers and stakeholders to design, test, and document improvements.
---

I joined the team responsible for a global financial messaging platform, in which payment messages move between dozens of services over Kafka. The other engineers were committed to finishing the release for the initial BIC, so my supervisor gave me a smaller problem and I worked largely on my own for the internship, with check-ins once every few days. This meant learning the codebase, the deployment setup, and the testing conventions without much hand-holding.

The platform had a "shadow runner" that replayed production-like traffic against a candidate release, but testers only had access to a single configuration. My task was to build a RESTful microservice in Scala using http4s and cats-effect that let testers define a scenario through an API: the message mix, the rate and ramp-up, and the duration. It could generate runs of several million messages, which it then launched, monitored, and reported on through endpoints for starting, pausing, and inspecting a run.

I documented the service with an API specification and testing overview, and I demonstrated it to the engineers and testers in the team at the end of the placement. Testers were then able to set up and manage a load experiment with far greater flexibility, and the team adopted the tool for its regular release testing runs.

**Skills:** Scala · Apache Kafka · REST APIs · Distributed Systems · Docker · Azure · Documentation · Independent Work