FROM registry.fedoraproject.org/fedora:rawhide
RUN dnf -y update
RUN dnf -y install texlive
RUN ls -l /usr/share/texlive/
RUN bash -c "test -w /usr/share/texlive/texmf-config/"
RUN test -w /usr/share/texlive/texmf-config/
