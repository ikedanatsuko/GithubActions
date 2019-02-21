FROM node:alpine

LABEL "com.github.actions.name"="GitHub Action for redoc-cli"
LABEL "com.github.actions.description"="Use redoc-cli"
LABEL "com.github.actions.icon"="package"
LABEL "com.github.actions.color"="purple"

LABEL "maintainer"="ikedanatsuko <ikedanatsuko@team-lab.com>"

RUN npm install -g redoc-cli

COPY "entrypoint.sh" "/entrypoint.sh"
RUN ["chmod","+x","/entrypoint.sh"]

ENTRYPOINT ["/entrypoint.sh"]