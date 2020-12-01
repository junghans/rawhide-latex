FROM registry.fedoraproject.org/fedora:rawhide
RUN echo "echo test" > test.sh
RUN chmod +x test.sh
RUN ls -l test.sh
RUN test -x test.sh
