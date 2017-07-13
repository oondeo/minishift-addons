# minishift-addons
Incubator for addons to minishift

## Install
You need to clone this repository and locate yourself on the root directory of your clone

````
git clone https://github.com/jorgemoralespou/minishift-addons.git
cd minishift-addons
````

## cors
An addon that will enable Cross-Origin resources from any source

## kubernetes-dashboard
An addon to install [kubernetes-dashboard](https://github.com/kubernetes/dashboard)

To access it:

````
minishift openshift service dashboard -n kube-dashboard
````

## cockpit
An addon to install [cockpit](http://cockpit-project.org/).

To access it:

````
minishift openshift service openshift-cockpit -n cockpit
````

# Install or enable
You need to install the addon:

````
minishift addons install <addon-name>
````

If you want to enable an addon once for your running minishift VM instance (if you have cloned this repo):

````
minishift addons apply <addon-name>
````

or permantently:

````
minishift addons enable <addon-name>
````

This will enable the addon everytime you create a new minishift VM instance.

