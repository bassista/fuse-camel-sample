# fuse-camel-sample
Fuse Camel Sample Project

    fabric:profile-edit --repositories mvn:com.ofbizian/features/1.0.0/xml/features default
    fabric:profile-create --parents feature-camel demo-profile
    container-create-child root demo-container
    container-add-profile demo-container demo-profile
    fabric:version-create --parent 1.0 --default 1.1
    fabric:profile-edit --features camel-ticket-service demo-profile 1.1
    container-upgrade --all 1.1
