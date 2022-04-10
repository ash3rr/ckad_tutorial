# ckad_tutorial
My Notes on the Kubernetes Certified Application Developer Course

# Volume Types

Volumes:
Volumes are defined in the Pod Spec. 
Defines the details of where and how the data is stored.

Volume Mounts:
Defined in the container spec.
Attaches the volume to a specific container.
Defines the path where the volume data will appear at runtime.

Types:
Hostpath is stored in a specific location directly on the host file system, on the kubernetes node where the Pod is running. (access host files from inside the container)

EmptyDir data is stored in an automatically managed location on the host file system. Data is deleted if the Pod is deleted. (deleted if the pod is deleted)

Persistent Volume Claim data is stored using a persistent volume (persists).

PersistentVolume:
Defines an abstract storage resource ready to be consumed by Pods. 
Defines details about the type and amount of storage provided.

PersistentVoumeClaim:
Defines the request to use the storage including details on the type of storage needed.
Automatically binds to an availavle PersistentVolume that meets the provided requirements.
Mounted to a Pod like a normal volume.

test