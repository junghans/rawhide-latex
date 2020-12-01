FROM registry.fedoraproject.org/fedora:rawhide
RUN dnf -y update
RUN dnf -y install git
RUN git clone https://github.com/votca/csg
RUN ls -l csg/share/scripts/inverse/prepare_generic.sh
RUN test -x csg/share/scripts/inverse/prepare_generic.sh
