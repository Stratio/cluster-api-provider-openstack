@Library('libpipelines@master') _

hose {
    EMAIL = 'eos@stratio.com'
    BUILDTOOL = 'make'
    VERSIONING_TYPE = 'stratioVersion-3-3'
    UPSTREAM_VERSION = '0.7.1'
    DEPLOYONPRS = true
    DEVTIMEOUT = 30
    ANCHORE_POLICY = "production"
    GRYPE_TEST = false

    DEV = { config ->
        doDocker(conf:config, dockerfile: 'Dockerfile', image:'cluster-api-provider-openstack')
    }
}