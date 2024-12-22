FROM FROM almalinux:9

ARG username
RUN adduser $username

USER $username
ARG project
ARG environmet
ARG team

RUN echo "Project: {$project} Environmet:{$environmet} Team: {$team}"

CMD ["sleep","120s"]