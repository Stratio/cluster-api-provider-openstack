@Library('libpipelines@master') _

hose {
    EMAIL = 'eos'
    BUILDTOOL = 'make'
    VERSIONING_TYPE = 'stratioVersion-3-3'
    UPSTREAM_VERSION = '2.0.2'
    DEPLOYONPRS = true
    DEVTIMEOUT = 30
    ANCHORE_POLICY = "production"
    GRYPE_TEST = false

    DEV = { config ->
        doUT(config)
        doDocker(config)
    }
}