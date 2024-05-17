# Restart Kubelet on Node

This script will restart kubelet on Node. Scenarios where a restart might be required:
- OpenShift related pod stuck in containerUnknown Status
- Certain bugs require container restart on Master Nodes. [Eg. https://access.redhat.com/solutions/6976343 ] 

- Add the node name as parameter.

## Usage

**ATTENTION** ⚠️ This script must only be used by the MCS (Managed Cloud Services) CRU (Crew Response Unit) team.
- If you need this script to be used, contact a MCS CRU member.
- The usage of this script is audited.
```
ocm backplane managedjob create CEE/restart-kubelet -p NODE="$NODE_NAME"
```

