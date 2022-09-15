FROM gcr.io/k8s-prow/clonerefs:v20220915-2520859b2c

# Commit details

ARG commit
ENV IMAGE_COMMIT=$commit
LABEL io.kyma-project.test-infra.commit=$commit

RUN mv /clonerefs /prow-clonerefs
COPY clonerefs /clonerefs
RUN chmod +x /clonerefs
