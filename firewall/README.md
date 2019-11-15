The bastion server here isn't routing traffic or serving as a full proxy, just a simple proxy that allows port 6443, 443, and 80 from external and serves the required internal ports for OpenShift on the internal side.

It's possible to add more proxy services or even routing to the bastion but really wasn't necessary.

My only concern is the bootstrap doesn't support the /healthz endpoint on port 6443 which meant abandoning my normal https healthchecks. Since this can be adjusted per host I'm considering defining those again but not checking the bootstrap node but this does depend on how the masters react to such a config.
