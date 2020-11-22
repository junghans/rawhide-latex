FROM registry.fedoraproject.org/fedora:rawhide
RUN dnf -y update
RUN dnf -y install texlive
RUN ls -l /usr/share/texlive/
RUN whoami
RUN test -w /usr/share/texlive/texmf-config/
