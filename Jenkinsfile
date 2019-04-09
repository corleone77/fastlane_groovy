@Library('nesbase@master') _


androidBuild {
    sonar['sonar.platform'] = 'stage'
    sonar['sonar.projectKey'] = 'android_shop'
    sonar['sonar.projectName'] = 'Android Shop'

    // Uncomment and update the value when a release from a branch other than develop is required
    // ReleaseBranch = 'release/january'

    BuildTypes = [
        debug  : [name: 'debug', flavorNames: ['store', 'stg']],
        release: [
            name       : 'release',
            flavorNames: [
                'dev',
                'dev2',
                'kraftwerk',
                'nesInt',
                'nesInt2',
                'nesInt3',
                'skunk',
                'stg',
                'rollout',
                'setup',
                'setup2',
                'nesTst',
                'prePrd'
            ]
        ]
    ]

    MavenProperties << [path: 'app/gradle.properties']

    Artifacts = [[
                    file: 'app/build/outputs/apk/${flavorName?.concat("/")?:""}${buildType}/*.apk',
                    type: 'apk'],
                [
                    file: 'app/build/outputs/mapping/${flavorName?.concat("/")?:""}${buildType}/mapping.txt',
                    type: 'mapping']
    ]

    previewRepo = "android-shop"
    previewServer = "nestor"
}


