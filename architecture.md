# Expectations for Architecture

## Separate Data Delivery from Presentation

The backends that deliver data, in reusable formats like JSON or XML, should be
completely separated from its presentation.

## Separate Configuration and Application

The application should be the same, no matter if it runs in dev, stage, test or
production. Only config should vary between environments.

## Build small and isolated Services

Services should only have one concern and solve that one concern really well.

## Build reactive architectures

Follow the [Reactive Manifesto](http://www.reactivemanifesto.org/).

## Build containerable apps

Follow the [12 Factor Manifesto](http://12factor.net/).

## Build pragmatic HTTP APIs

~~Follow our [[/w/best_practice/api_design_and_development/ | best practices for
pragmatic APIs]].~~

Follow [Best Practices for Designing a Pragmatic RESTful
API](http://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api).

## Generic remarks

Read up on [PHP: The Right Way](http://www.phptherightway.com/).
