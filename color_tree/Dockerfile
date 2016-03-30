FROM ruby:2.3-alpine

MAINTAINER Ryan Moore <moorer@udel.edu>

RUN gem install \
    abort_if \
    bio \
    parse_fasta \
    trollop

RUN \curl -sSL https://github.com/mooreryan/color_tree/archive/v0.6.0.tar.gz \
    | tar -v -C /usr/src -xz

ENV PATH /usr/src/color_tree-0.6.0:$PATH

CMD ["color_tree", "--help"]
