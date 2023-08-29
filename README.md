# Orb Template

circleci setup

create `dev` context with `CIRCLE_TOKEN` env var

circleci namespace create xavidop github  xavidop

circleci orb init .

circleci orb pack ./src > orb.yml

circleci orb publish orb.yml circleci/ORB_NAME@dev:alpha

circleci orb publish promote circleci/ORB_NAME@dev:alpha patch

