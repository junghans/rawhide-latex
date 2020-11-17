FROM registry.fedoraproject.org/fedora:rawhide
RUN dnf -y update
RUN dnf -y install texlive
RUN ls -l /usr/bin/kpsewhich
RUN ldd /usr/bin/kpsewhich
RUN ls -l /usr/share/texlive/texmf-dist/ls-R
RUN kpsewhich -debug 2 fmtutil.cnf
RUN cat /usr/share/texlive/texmf-dist/web2c/fmtutil.cnf
RUN /usr/bin/fmtutil-sys --all || :
RUN printf '\\documentclass{article}\n\\begin{document}\ntest\n\\end{document}' > test.tex
RUN latex test.tex
