# Staff Infrastructure Interview Take Home Exercise


## Objective

Describe how you would approach designing and implementing infrastructure
solutions for a highly regulated, multi-cloud, multi-region web application.

Imagine a scenario where you are tasked with leading an effort to build out
infrastructure for a new backend services in the United States. Each state has
its own rules and regulations. This usually means requests must be processed and
customer data must be stored on hardware located physically within a given
state’s borders. Your assignment is to come up with a high level plan and present
it to a panel of interviewers.

## Deliverables

* Feel free to use whatever presentation methods you are comfortable with (powerpoint, architecture diagrams, outlines, etc.).

* The backend services run in containers orchestrated by Kubernetes. Your plan
should include considerations for operating and maintaining Kubernetes in a hybrid
cloud environment, which Kubernetes distribution will be used and why, as well as
underlying hardware and any off-the-shelf software.

* The backend services could be a mix of different languages, including Ruby and
.NET. Other requirements for the stack include a Postgres database, Redis cache,
and RabbitMQ for message brokering.

* Choosing a single cloud provider likely won’t work, as you must account for running
services and databases across multiple states, and it is unlikely one provider
has data centers in all states. Some states may have no public cloud presence whatsoever.

* Due to some states not having public cloud presence, you will likely have to
account for leasing rack space from colocation data centers, sourcing hardware,
configuring network access, etc. We’d love to hear about your approach to this,
and/or pros and cons of different approaches.

* Beyond basic networking, present how you would implement a “single pane of glass”
approach to observability in order to gain an accurate view of all deployed clusters.
