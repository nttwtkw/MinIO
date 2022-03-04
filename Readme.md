# MinIO 3.4.7
helm install --namespace minio --set nameOverride=minio,fullnameOverride=minio,rootUser=rootuser,rootPassword=rootpass123,replicas=4,persistence.storageClass=rook-cephfs,persistence.size=100Gi,consoleService.type=NodePort,resources.requests.memory=1Gi --generate-name minio/minio --debug
