Shopping Cart Application DevOps

Code changes that are committed to Git start the process by starting the CI/CD pipeline. The pipeline's initial step is on assembling the source code and running Maven unit tests to make sure the code is dependable and functioning. A comprehensive code quality check is carried out using SonarQube after compilation and testing are completed successfully. By locating and eliminating any code vulnerabilities, this phase improves the application's overall security and maintainability.

In order to find vulnerabilities in the application's dependencies, OWASP Dependency-Check is utilized. This aids in addressing possible dangers related to third-party components and libraries. Following the completion of these security and quality checks, the application and its dependencies are once more built and packaged using Maven into a distributable artifact.

Following that, the artifact is saved in Nexus Repository Manager, a secure and efficient repository for build artifact management. The next step is creating a Docker image from the bundled asset. Aqua Trivy is used to scan the image for vulnerabilities before releasing it to the Docker registry. This stage ensures that any security problems in the image are identified and corrected before deployment.

Finally, the Docker image is deployed to an Amazon Web Services Kubernetes cluster. Deploying on the cloud enables efficient and scalable application management. The project aims to combine DevOps ideas and tools to develop a safe and constantly deployable cloud-based application that demonstrates the efficacy of modern DevOps techniques.
