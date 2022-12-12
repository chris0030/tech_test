# tech_test

## Approach

I will take the approach of setting up a CentOS development server on my home rack
and use this to set up and test a bash script capable of performing the following tasks.
I will use Version Control to store and present the script, and once it's tested and I'm
happy. I will use scp to copy the script to the server and run it.

## Negatives of this approach

Without overly complex scripting, which is out of scope for the timing of this test, 
the bash script will be imperative and thus not idempotent.

## Notes

- CentOS 7

`ssh –i test-linux-temp.pem centos@nn.nn.nn.nn`