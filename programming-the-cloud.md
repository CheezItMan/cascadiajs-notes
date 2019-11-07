# Programming the Cloud with JS

Christian Nunciato
@cnunciato

Works at Pulumi
Worked at Chef

Studied film

## What this is

- Infrastructure as Code
- Managing my own infrastructure
  - Beyond Heroku
- representing server stuff as code


## Heroku

Problems:

1.  Can't see what's inside, 
2.  can't duplicate it, 
3.  can't scale it out easily
4.  Can't recover from problems

### Tools of infrastructure as code

- Chef set of recipies to set things up.  Config management tools
  - Chef (ruby)
  - Puppet
  - Ansible (yaml)
  - Saltstack (Yaml)
- Provisioning tools
  - Point it at a cloud and it builds things
    - Use it to spin up virtual infrastructure and Chef or something to set it up.


Things they have in common

- Declaritive
- Idempotent - Given the same code as input you'll get the same result.

Good:

- Reliable
- repeatable
- Replicable
- Testable
- Self documenting

We haven't been shown how to build infrastructure as code.

We need abstractions to rise to meet us to where we are.






