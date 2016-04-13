FROM ruby:2.3

MAINTAINER Ryan Moore <moorer@udel.edu>

RUN gem install bundler



RUN \curl -sSL https://github.com/mooreryan/ZetaHunter/archive/v0.0.3-alpha.tar.gz \
    | tar -v -C /home -xz

RUN bundle install --gemfile /home/ZetaHunter-0.0.3-alpha/Gemfile

CMD ["ruby", "/home/ZetaHunter-0.0.3-alpha/zeta_hunter.rb", "--help"]
