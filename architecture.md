# Expectations for Architecture

## A. Separate Data Delivery from Presentation

The backends that deliver data, in reusable formats like JSON or XML, should be
completely separated from its presentation.

## B. Separate Configuration and Application

The application should be the same, no matter if it runs in dev, stage, test or
production. Only config should vary between environments.

## C. Build small and isolated Services

Services should only have one concern and solve that one concern really well.

## D. Build reactive architectures

Follow the [[http://www.reactivemanifesto.org/ | Reactive Manifesto]].

## E. Build containerable apps

Follow the [[ http://12factor.net/ | 12 Factor Manifesto ]].

## F. Build pragmatic HTTP APIs

Follow our [[/w/best_practice/api_design_and_development/ | best practices for
pragmatic APIs]].

## G. Generic remarks

Read up on [[http://www.phptherightway.com/ | PHP: The Right Way]].
