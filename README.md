# Orb Template

https://circleci.com/docs/creating-orbs/

circleci setup

create `dev` context with `CIRCLE_TOKEN` env var

circleci namespace create xavidop github xavidop
Settings -> Security -> Allow uncertified orbs
circleci orb create xavidop/circleci-orb-hello-world

circleci orb init .

circleci orb pack ./src > orb.yml

circleci orb publish orb.yml circleci/ORB_NAME@dev:alpha

circleci orb publish promote circleci/ORB_NAME@dev:alpha patch

