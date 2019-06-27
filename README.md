This is a file_roots based template, for Hubblestack, for configuring host based "pillar data" for custom things not worth checking into the main pillar data repository (https://github.com/craftypenguins/hubblestack_data). 

The topfile for Nova and Pulsar assumes these yaml files exist and that this directory is set as file_roots (not pillar_roots, custom pillar parsing in hubble) in /etc/hubble/hubble. It breaks if there isn't something to parse, so a generic check for hubble running and an /etc/ declaration that does nothing is included.
