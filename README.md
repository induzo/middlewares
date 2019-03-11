# Useful Go HTTP middlewares

[![Documentation](https://godoc.org/github.com/induzo/gohttpmw?status.svg)](http://godoc.org/github.com/induzo/gohttpmw) [![Go Report Card](https://goreportcard.com/badge/github.com/induzo/gohttpmw)](https://goreportcard.com/report/github.com/induzo/gohttpmw) [![Coverage Status](https://coveralls.io/repos/github/induzo/gohttpmw/badge.svg?branch=master)](https://coveralls.io/github/induzo/gohttpmw?branch=master) [![CircleCI](https://circleci.com/gh/induzo/gohttpmw.svg?style=svg)](https://circleci.com/gh/induzo/gohttpmw) [![Maintainability](https://api.codeclimate.com/v1/badges/9f9a4038e01e79fbd5be/maintainability)](https://codeclimate.com/github/induzo/gohttpmw/maintainability)

## Content type

Simply set the content-type in the header.

## RBAC

depends on

- github.com/ory/ladon

Allows to check if a user is allowed to access the URL, according to his role.
You need to specify the function that will get the role name from the context.

## Request ID

depends on

- github.com/rs/xid

Set a request id in the context as well as the header.

## Security

Set the basic headers necessary for a better security.
These are not sufficient, you will need to add more according to the context of your application.

## Logger

If you want performance, use LoggerZero.
Otherwise, simply use logrus.
Add logs to the request
_If you use other middlewares, make sure they don't change the reference to the request_
