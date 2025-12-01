# [Command] _network network-watcher flow-log create_

Create a flow log for the specified network security group.

## Versions

### [2025-03-01](/Resources/mgmt-plane/L3N1YnNjcmlwdGlvbnMve30vcmVzb3VyY2Vncm91cHMve30vcHJvdmlkZXJzL21pY3Jvc29mdC5uZXR3b3JrL25ldHdvcmt3YXRjaGVycy97fS9mbG93bG9ncy97fQ==/2025-03-01.xml) **Stable**

<!-- mgmt-plane /subscriptions/{}/resourcegroups/{}/providers/microsoft.network/networkwatchers/{}/flowlogs/{} 2025-03-01 -->

#### examples

- Create or update flow log
    ```bash
        network network-watcher flow-log create --resource-group rg1 --network-watcher-name nw1 --flow-log-name fl --location centraluseuap --target-resource-id /subscriptions/subid/resourceGroups/rg1/providers/Microsoft.Network/networkSecurityGroups/desmondcentral-nsg --storage-id /subscriptions/subid/resourceGroups/rg1/providers/Microsoft.Storage/storageAccounts/nwtest1mgvbfmqsigdxe --enabled-filtering-criteria srcIP=158.255.7.8 || dstPort=56891 --record-types B,E --enabled True --format "{type:JSON,version:1}" --type UserAssigned --user-assigned-identities "{/subscriptions/subid/resourceGroups/rg1/providers/Microsoft.ManagedIdentity/userAssignedIdentities/id1:{}}"
    ```
