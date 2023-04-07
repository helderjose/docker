FROM fedora:35

# para executar o comando nvm
SHELL ["/bin/bash", "--login", "-c"]

RUN dnf install -y git-all && dnf clean all

# instalacao node
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash
RUN source ~/.bashrc
RUN nvm install v10.24.1
RUN nvm alias default v10.24.1

# instalacao vue
RUN npm install -g @vue/cli@4.4.5 @vue/cli-service-global




# WORKDIR /
# EXPOSE 8080
# VOLUME $(pwd):/home/diagnostic-new
# VOLUME $(pwd) /home/diagnostic-new
# VOLUME . /home/diagnostic-new


# docker build -t diagnostic-new-image .
# docker container run -it -p 8080:8080 -v $(pwd):/home/diagnostic-new --name diagnostic-new diagnostic-new-image bash

# docker container start diagnostic-new
# docker container exec -it diagnostic-new bash
# docker container exec -it diagnostic-new bash && cd /home/diagnostic-new




# docorm -f diagnostic-new && doimgrm diagnostic-new-image
