FROM archlinux/base:latest

COPY arch-mirrorlist /etc/pacman.d/mirrorlist

RUN pacman-key --init && \
    pacman -Syyu --noconfirm && \
    pacman -S --noconfirm base-devel

RUN useradd -ms /bin/bash builduser
RUN echo "builduser ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builduser

USER builduser
ENTRYPOINT ["/bin/bash"]