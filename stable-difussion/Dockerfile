FROM archlinux:latest
RUN pacman -Sy wget git python3
# RUN if [ $(getent group $GID) ]; then groupdel -f `getent group $GID | cut -d: -f1`; fi \
#   && if [ $(getent passwd $UID) ]; then userdel -f `getent passwd $UID | cut -d: -f1`; fi \
#   && groupadd -r user -g $GID \
#   && useradd -d /home/user -u $UID -m -s /bin/bash -g user user \
#   && chown -R user:user /home/user
# USER user
WORKDIR /home/user
CMD ["./webui.sh"]
