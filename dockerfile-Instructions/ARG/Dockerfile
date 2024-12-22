FROM FROM almalinux:9

ARG username
RUN adduser $username

USER $username
ARG PROJECT
ARG ENVIRONMENT
ARG TEAM
ENV PROJECT = ${PROJECT}
ENV ENVIRONMENT = ${ENVIRONMENT}
ENV TEAM = ${TEAM}

RUN echo "Project: ${PROJECT} Environmet:${ENVIRONMENT} Team: ${TEAM}"

CMD ["sleep","120"]