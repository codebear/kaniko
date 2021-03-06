# v0.16.0 Release - 2020-01-17

Happy New Year 2020!

## Bug Fixes
* Support for private registries in the cache warmer [#941](https://github.com/GoogleContainerTools/kaniko/pull/941)
* Fix bug with docker compatibility ArgsEscaped [#964](https://github.com/GoogleContainerTools/kaniko/pull/964)
* Clean code (Condition is always 'false' because 'err' is always 'nil' ). [#967](https://github.com/GoogleContainerTools/kaniko/pull/967)
* Fix #647 Copy dir permissions [#961](https://github.com/GoogleContainerTools/kaniko/pull/961)
* Allow setting serviceAccount in integration test [#965](https://github.com/GoogleContainerTools/kaniko/pull/965)
* Fix #926 cache warmer and method signature [#927](https://github.com/GoogleContainerTools/kaniko/pull/927)
* Fix #948 update valid license years [#949](https://github.com/GoogleContainerTools/kaniko/pull/949)
* Move hash bang to first line. [#954](https://github.com/GoogleContainerTools/kaniko/pull/954)
* Fix #944 include docker-credential-acr-linux [#945](https://github.com/GoogleContainerTools/kaniko/pull/945)
* Fix #925 broken insecure pull [#932](https://github.com/GoogleContainerTools/kaniko/pull/932)
* Push to ECR using instance roles [#930](https://github.com/GoogleContainerTools/kaniko/pull/930)
* Upgrade aws go sdk for supporting eks oidc credential chain [#832](https://github.com/GoogleContainerTools/kaniko/pull/832)
* Push image [#866](https://github.com/GoogleContainerTools/kaniko/pull/866)

# Updates and Refactors
* Fixes #950 integration test failing on go 1.13 [#955](https://github.com/GoogleContainerTools/kaniko/pull/955)
* Tidy dependencies [#939](https://github.com/GoogleContainerTools/kaniko/pull/939)
* changing to modules from dependencies [#869](https://github.com/GoogleContainerTools/kaniko/pull/869)
* Changing Log to trace [#920](https://github.com/GoogleContainerTools/kaniko/pull/920)

# Documentation
* docs: fix document on DoBuild [#668](https://github.com/GoogleContainerTools/kaniko/pull/668)
* Update outdated toc in README.md [#867](https://github.com/GoogleContainerTools/kaniko/pull/867)

Huge thank you for this release towards our contributors:
- Adrian Mouat
- Balint Pato
- Ben Einaudi
- Benjamin EINAUDI
- Carlos Sanchez
- Cole Wippern
- Daniel Strobusch
- Eduard Laur
- Fahri Yardımcı
- Josh Soref
- lou-lan
- Nao YONASHIRO
- poy
- Prashant Arya
- priyawadhwa
- Pweetoo
- Remko van Hunen
- Sam Stoelinga
- Stijn De Haes
- Tejal Desai
- tommaso.doninelli
- Will Ripley


# v0.15.0 Release - 2019-12-20

## Bug fixes
* Fix #899 cached copy results in inconsistent key [#914](https://github.com/GoogleContainerTools/kaniko/pull/914)
* Fix contribution issue sentence [#912](https://github.com/GoogleContainerTools/kaniko/pull/912)
* Include source stage cache key in cache key for COPY commands using --from [#883](https://github.com/GoogleContainerTools/kaniko/pull/883)
* Fix failure when using capital letters in image alias in 'FROM ... AS…' instruction [#839](https://github.com/GoogleContainerTools/kaniko/pull/839)
* Add golangci.yaml file matching current config [#893](https://github.com/GoogleContainerTools/kaniko/pull/893)
* when copying, skip files with the same name [#905](https://github.com/GoogleContainerTools/kaniko/pull/905)
* Modified error message for writing image with digest file [#849](https://github.com/GoogleContainerTools/kaniko/pull/849)
* Don't exit optimize early; record last cachekey [#892](https://github.com/GoogleContainerTools/kaniko/pull/892)
* Final cachekey for stage [#891](https://github.com/GoogleContainerTools/kaniko/pull/891)
* Update error handling and logging for cache [#879](https://github.com/GoogleContainerTools/kaniko/pull/879)
* Resolve symlink targets to abs path before copying [#857](https://github.com/GoogleContainerTools/kaniko/pull/857)
* Fix quote strip behavior for ARG values [#850](https://github.com/GoogleContainerTools/kaniko/pull/850)

## Updates and Refactors
* add unit tests for caching run and copy [#888](https://github.com/GoogleContainerTools/kaniko/pull/888)
* Only build required docker images for integration tests [#898](https://github.com/GoogleContainerTools/kaniko/pull/898)
* Add integration test for add url with arg [#863](https://github.com/GoogleContainerTools/kaniko/pull/863)
* Add unit tests for compositecache and stagebuilder [#890](https://github.com/GoogleContainerTools/kaniko/pull/890)

## Documentation
* updated readme [#906](https://github.com/GoogleContainerTools/kaniko/pull/906)
* nits in README [#861](https://github.com/GoogleContainerTools/kaniko/pull/861)
* Invalid link to missing file config.json [#876](https://github.com/GoogleContainerTools/kaniko/pull/876)
* Fix README.md anchor links [#872](https://github.com/GoogleContainerTools/kaniko/pull/872)
* Update readme known issues [#874](https://github.com/GoogleContainerTools/kaniko/pull/874)

Huge thank you for this release towards our contributors:
- Balint Pato
- Ben Einaudi
- Cole Wippern
- Eduard Laur
- Josh Soref
- Pweetoo
- Tejal Desai
- Will Ripley
- poy
- priyawadhwa
- tommaso.doninelli


# v0.14.0 Release - 2019-11-08

## New Features
* Added --image-name-with-digest flag [#841](https://github.com/GoogleContainerTools/kaniko/pull/841)
* Add support to download context file from Azure Blob Storage [#816](https://github.com/GoogleContainerTools/kaniko/pull/816)
* Add BUILD_ARGs to ease use of proxy [#810](https://github.com/GoogleContainerTools/kaniko/pull/810)

## Bug Fixes
* fix tests for default home [#824](https://github.com/GoogleContainerTools/kaniko/pull/824)
* Issue #439 Strip out double quotes in ARG value [#834](https://github.com/GoogleContainerTools/kaniko/pull/834)
* Fixes caching with COPY command [#773](https://github.com/GoogleContainerTools/kaniko/pull/773)
* 828: clean up docker doc, fix context var in run cmd [#829](https://github.com/GoogleContainerTools/kaniko/pull/829)
* fix build_args in MakeFile, have Travis run make images to preven issue in future [#821](https://github.com/GoogleContainerTools/kaniko/pull/821)

## Updates and Refactors
* changing debug to trace [#825](https://github.com/GoogleContainerTools/kaniko/pull/825)

## Documentation
* Details about --tarPath usage improved [#811](https://github.com/GoogleContainerTools/kaniko/pull/811)


# v0.13.0 Release - 2019-10-04

## New Features
* Add `kaniko version` command [#796](https://github.com/GoogleContainerTools/kaniko/pull/796)
* Write data about pushed images for GCB kaniko build step if env var `BUILDER_OUTPUT` is set [#602](https://github.com/GoogleContainerTools/kaniko/pull/602)
* Support `Dockerfile.dockerignore` relative to `Dockerfile` [#801](https://github.com/GoogleContainerTools/kaniko/pull/801)

## Bug Fixes
* fix creating abs path for urls [#804](https://github.com/GoogleContainerTools/kaniko/pull/804)
* Fix #691 - ADD does not understand ENV variables [#768](https://github.com/GoogleContainerTools/kaniko/pull/768)
* Resolve relative paths to absolute paths in command line arguments [#736](https://github.com/GoogleContainerTools/kaniko/pull/736)
* insecure flag is now honored with `--cache` flag. [#685](https://github.com/GoogleContainerTools/kaniko/pull/685)
* Reduce log level for adding file message [#624](https://github.com/GoogleContainerTools/kaniko/pull/624)
* Fix SIGSEGV on file system deletion while building [#765](https://github.com/GoogleContainerTools/kaniko/pull/765)

## Updates and Refactors
* add debug level info what is the layer type [#805](https://github.com/GoogleContainerTools/kaniko/pull/805)
* Update base image to golang:1.12 [#648](https://github.com/GoogleContainerTools/kaniko/pull/648)
* Add some triage notes to issue template. [#794](https://github.com/GoogleContainerTools/kaniko/pull/794)
* double help text about skip-verify-tls [#782](https://github.com/GoogleContainerTools/kaniko/pull/782)
* Add a pull request template [#795](https://github.com/GoogleContainerTools/kaniko/pull/795)
* Correct CheckPushPermission comment. [#671](https://github.com/GoogleContainerTools/kaniko/pull/671)

## Documentation
* Use kaniko with docker config.json password [#129](https://github.com/GoogleContainerTools/kaniko/pull/129)
* Add getting started tutorial [#790](https://github.com/GoogleContainerTools/kaniko/pull/790)

## Performance
* feat: optimize build [#694](https://github.com/GoogleContainerTools/kaniko/pull/694)

Huge thank you for this release towards our contributors: 
- alexa
- Andreas Bergmeier
- Carlos Alexandro Becker
- Carlos Sanchez
- chhsia0
- debuggy
- Deniz Zoeteman
- Don McCasland
- Fred Cox
- Herrmann Hinz
- Hugues Alary
- Jason Hall
- Johannes 'fish' Ziemke
- jonjohnsonjr
- Luke Wood
- Matthew Dawson
- Mingliang Tao
- Monard Vong
- Nao YONASHIRO
- Niels Denissen
- Prashant
- priyawadhwa
- Priya Wadhwa
- Sascha Askani
- sharifelgamal
- Sharif Elgamal
- Takeaki Matsumoto
- Taylor Barrella
- Tejal Desai
- Thao-Nguyen Do
- tralexa
- Victor Noel
- v.rul
- Warren Seymour
- xanonid
- Xueshan Feng
- Антон Костенко
- Роман Небалуев

# v0.12.0 Release - 2019-09/13

## New Features
* Added `--oci-layout-path` flag to save image in OCI layout. [#744](https://github.com/GoogleContainerTools/kaniko/pull/744)
* Add support for S3 custom endpoint [#698](https://github.com/GoogleContainerTools/kaniko/pull/698)

## Bug Fixes
* Setting PATH [#760](https://github.com/GoogleContainerTools/kaniko/pull/760)
* Remove leading slash in layer tarball paths (Closes: #726) [#729](https://github.com/GoogleContainerTools/kaniko/pull/729)

## Updates and Refactors
* Remove cruft [#635](https://github.com/GoogleContainerTools/kaniko/pull/635)
* Add desc for `--skip-tls-verify-pull` to README [#493](https://github.com/GoogleContainerTools/kaniko/pull/493)

Huge thank you for this release towards our contributors: 
- Carlos Alexandro Becker
- Carlos Sanchez
- chhsia0
- Deniz Zoeteman
- Luke Wood
- Matthew Dawson
- Niels Denissen
- Priya Wadhwa
- Sharif Elgamal
- Takeaki Matsumoto
- Taylor Barrella
- Tejal Desai
- v.rul
- Warren Seymour
- xanonid
- Xueshan Feng
- Роман Небалуев


# v0.11.0 Release - 2019-08-23

## Bug Fixes
* fix unpacking archives via ADD [#717](https://github.com/GoogleContainerTools/kaniko/pull/717)
* Reverted not including build args in cache key [#739](https://github.com/GoogleContainerTools/kaniko/pull/739)
* Create cache directory if it doesn't already exist [#452](https://github.com/GoogleContainerTools/kaniko/pull/452)

## New Features
* add multiple user agents to kaniko if upstream_client_type value  is set [#750](https://github.com/GoogleContainerTools/kaniko/pull/750)
* Make container layers captured using FS snapshots reproducible [#714](https://github.com/GoogleContainerTools/kaniko/pull/714)
* Include warmer in debug image [#497](https://github.com/GoogleContainerTools/kaniko/pull/497)
* Bailout when there is not enough input arguments [#735](https://github.com/GoogleContainerTools/kaniko/pull/735)
* Add checking image presence in cache prior to downloading it [#723](https://github.com/GoogleContainerTools/kaniko/pull/723)

## Additonal PRs
* Document how to build from git reference [#730](https://github.com/GoogleContainerTools/kaniko/pull/730)
* Misc. small changes/refactoring [#712](https://github.com/GoogleContainerTools/kaniko/pull/712)
* Update go-containerregistry [#680](https://github.com/GoogleContainerTools/kaniko/pull/680)
* Update version of go-containerregistry [#724](https://github.com/GoogleContainerTools/kaniko/pull/724)
* feat: support specifying branch for cloning [#703](https://github.com/GoogleContainerTools/kaniko/pull/703)

Huge thank you for this release towards our contributors: 
- Carlos Alexandro Becker
- Carlos Sanchez
- Deniz Zoeteman
- Luke Wood
- Matthew Dawson
- priyawadhwa
- sharifelgamal
- Sharif Elgamal
- Taylor Barrella
- Tejal Desai
- v.rul
- Warren Seymour
- Xueshan Feng
- Роман Небалуе

# v0.10.0 Release - 2019-06-19

## Bug Fixes
* Fix kaniko caching [#639](https://github.com/GoogleContainerTools/kaniko/pull/639)
* chore: fix typo [#665](https://github.com/GoogleContainerTools/kaniko/pull/665)
* Fix file mode bug [#618](https://github.com/GoogleContainerTools/kaniko/pull/618)
* Fix arg handling for multi-stage images in COPY instructions. [#621](https://github.com/GoogleContainerTools/kaniko/pull/621)
* Fix parent directory permissions [#619](https://github.com/GoogleContainerTools/kaniko/pull/619)
* Environment variables should be replaced in URLs in ADD commands. [#580](https://github.com/GoogleContainerTools/kaniko/pull/580)
* Update the cache warmer to also save manifests. [#576](https://github.com/GoogleContainerTools/kaniko/pull/576)
* Fix typo in error message [#569](https://github.com/GoogleContainerTools/kaniko/pull/569)

## New Features
* Add SkipVerify support to CheckPushPermissions. [#663](https://github.com/GoogleContainerTools/kaniko/pull/663)
* Creating  github Build Context [#672](https://github.com/GoogleContainerTools/kaniko/pull/672)
* Add `--digest-file` flag to output built digest to file. [#655](https://github.com/GoogleContainerTools/kaniko/pull/655)
* README.md: update BuildKit/img comparison [#642](https://github.com/GoogleContainerTools/kaniko/pull/642)
* Add documentation for --verbosity flag [#634](https://github.com/GoogleContainerTools/kaniko/pull/634)
* Optimize file copying and stage saving between stages. [#605](https://github.com/GoogleContainerTools/kaniko/pull/605)
* Add an integration test for USER unpacking. [#600](https://github.com/GoogleContainerTools/kaniko/pull/600)
* Added missing documentation for --skip-tls-verify-pull arg [#593](https://github.com/GoogleContainerTools/kaniko/pull/593)
* README.me: update Buildah description [#586](https://github.com/GoogleContainerTools/kaniko/pull/586)
* Add missing tests for bucket util [#565](https://github.com/GoogleContainerTools/kaniko/pull/565)
* Look for manifests in the local cache next to the full images. [#570](https://github.com/GoogleContainerTools/kaniko/pull/570)
* Make the run_in_docker script support caching. [#564](https://github.com/GoogleContainerTools/kaniko/pull/564)
* Refactor snapshotting [#561](https://github.com/GoogleContainerTools/kaniko/pull/561)
* Stop storing a separate cache hash. [#560](https://github.com/GoogleContainerTools/kaniko/pull/560)
* Speed up workdir by always returning an empty filelist (rather than a… [#557](https://github.com/GoogleContainerTools/kaniko/pull/557)
* Refactor whitelist handling. [#559](https://github.com/GoogleContainerTools/kaniko/pull/559)
* Refactor the build loop to fetch stagebuilders earlier. [#558](https://github.com/GoogleContainerTools/kaniko/pull/558)

## Additonal PRs
* Improve changelog dates [#657](https://github.com/GoogleContainerTools/kaniko/pull/657)
* Change verbose output from info to debug [#640](https://github.com/GoogleContainerTools/kaniko/pull/640)
* Check push permissions before building images [#622](https://github.com/GoogleContainerTools/kaniko/pull/622)
* Bump go-containerregistry to 8c1640add99804503b4126abc718931a4d93c31a [#609](https://github.com/GoogleContainerTools/kaniko/pull/609)
* Update go-containerregistry [#599](https://github.com/GoogleContainerTools/kaniko/pull/599)
* Log "Skipping paths under..." to debug [#571](https://github.com/GoogleContainerTools/kaniko/pull/571)

Huge thank you for this release towards our contributors: 
- Achilleas Pipinellis
- Adrian Duong
- Akihiro Suda
- Andreas Bergmeier
- Andrew Rynhard
- Anthony Weston
- Anurag Goel
- Balint Pato
- Christie Wilson
- Daisuke Taniwaki
- Dan Cecile
- Dirk Gustke
- dlorenc
- Fredrik Lönnegren
- Gijs
- Jake Shadle
- James Rawlings
- Jason Hall
- Johan Hernandez
- Johannes 'fish' Ziemke
- Kartik Verma
- linuxshokunin
- MMeent
- Myers Carpenter
- Nándor István Krácser
- Nao YONASHIRO
- Priya Wadhwa
- Sharif Elgamal
- Shuhei Kitagawa
- Valentin Rothberg
- Vincent Demeester

# v0.9.0 Release - 2019-02-08

## Bug Fixes
* Bug fix with volumes declared in base images during multi-stage builds
* Bug fix during snapshotting multi-stage builds.
* Bug fix for caching with tar output.

# v0.8.0 Release - 2019-01-29

## New Features
* Even faster snapshotting with godirwalk
* Added TTL for caching

## Updates
* Change cache key calculation to be more reproducible.
* Make the Digest calculation faster for locally-cached images.
* Simplify snapshotting.

## Bug Fixes
* Fix bug with USER command and unpacking base images.
* Added COPY --from=previous stage name/number validation

# v0.7.0 Release - 2018-12-10

## New Features
* Add support for COPY --from an unrelated image

## Updates
* Speed up snapshotting by using filepath.SkipDir
* Improve layer cache upload performance
* Skip unpacking the base image in certain cases

## Bug Fixes
* Fix bug with call loop
* Fix caching for multi-step builds

# v0.6.0 Release - 2018-11-06

## New Features
* parse arg commands at the top of dockerfiles [#404](https://github.com/GoogleContainerTools/kaniko/pull/404)
* Add buffering for large layers. [#428](https://github.com/GoogleContainerTools/kaniko/pull/428)
* Separate Insecure Pull Options [#409](https://github.com/GoogleContainerTools/kaniko/pull/409)
* Add support for .dockerignore file [#394](https://github.com/GoogleContainerTools/kaniko/pull/394)
* Support insecure pull [#401](https://github.com/GoogleContainerTools/kaniko/pull/401)

## Updates
* Preserve options when doing a cache push [#423](https://github.com/GoogleContainerTools/kaniko/pull/423)
* More cache cleanups: [#397](https://github.com/GoogleContainerTools/kaniko/pull/397)
*  adding documentation for base image caching [#421](https://github.com/GoogleContainerTools/kaniko/pull/421)
* Update go-containerregistry [#420](https://github.com/GoogleContainerTools/kaniko/pull/420)
* Update README [#419](https://github.com/GoogleContainerTools/kaniko/pull/419)
* Use remoteImage function when getting digest for cache [#413](https://github.com/GoogleContainerTools/kaniko/pull/413)
* adding exit 1 when there are not enough command line vars passed to `… [#415](https://github.com/GoogleContainerTools/kaniko/pull/415)
* "Container Builder" - > "Cloud Build" [#414](https://github.com/GoogleContainerTools/kaniko/pull/414)
* adding the cache warmer to the release process [#412](https://github.com/GoogleContainerTools/kaniko/pull/412)

## Bug Fixes
* Fix bugs with .dockerignore and improve integration test [#424](https://github.com/GoogleContainerTools/kaniko/pull/424)
* fix releasing the cache warmer [#418](https://github.com/GoogleContainerTools/kaniko/pull/418)


# v0.5.0 Release - 2018-10-16

## New Features
* Persistent volume caching for base images [#383](https://github.com/GoogleContainerTools/kaniko/pull/383)

## Updates
* Use only the necessary files in the cache keys. [#387](https://github.com/GoogleContainerTools/kaniko/pull/387)
* Change loglevel for copying files to debug (#303) [#393](https://github.com/GoogleContainerTools/kaniko/pull/393)
* Improve IsDestDir functionality with filesystem info [#390](https://github.com/GoogleContainerTools/kaniko/pull/390)
* Refactor the build loop. [#385](https://github.com/GoogleContainerTools/kaniko/pull/385)
* Rework cache key generation a bit. [#375](https://github.com/GoogleContainerTools/kaniko/pull/375)

## Bug Fixes
* fix mispell [#396](https://github.com/GoogleContainerTools/kaniko/pull/396)
* Update go-containerregistry dependency [#388](https://github.com/GoogleContainerTools/kaniko/pull/388)
* chore: fix broken markdown (CHANGELOG.md) [#382](https://github.com/GoogleContainerTools/kaniko/pull/382)
* Don't cut everything after an equals sign [#381](https://github.com/GoogleContainerTools/kaniko/pull/381)


# v0.4.0 Release - 2018-10-01

## New Features
* Add a benchmark package to store and monitor timings. [#367](https://github.com/GoogleContainerTools/kaniko/pull/367)
* Add layer caching to kaniko [#353](https://github.com/GoogleContainerTools/kaniko/pull/353)
* Update issue templates [#340](https://github.com/GoogleContainerTools/kaniko/pull/340)
* Separate --insecure-skip-tls-verify flag into two separate flags [#311](https://github.com/GoogleContainerTools/kaniko/pull/311)
* Updated created by time for built image [#328](https://github.com/GoogleContainerTools/kaniko/pull/328)
* Add Flag to Disable Push to Container Registry [#292](https://github.com/GoogleContainerTools/kaniko/pull/292)
* Add a new flag to cleanup the filesystem at the end [#370](https://github.com/GoogleContainerTools/kaniko/pull/370)

## Updates
* Update README to add information about layer caching [#364](https://github.com/GoogleContainerTools/kaniko/pull/364)
* Suppress usage upon Run error [#356](https://github.com/GoogleContainerTools/kaniko/pull/356)
* Refactor build into stageBuilder type [#343](https://github.com/GoogleContainerTools/kaniko/pull/343)
* Replace gometalinter with GolangCI-Lint [#349](https://github.com/GoogleContainerTools/kaniko/pull/349)
* Add Key() to LayeredMap and Snapshotter [#337](https://github.com/GoogleContainerTools/kaniko/pull/337)
* Add CacheCommand to DockerCommand interface [#336](https://github.com/GoogleContainerTools/kaniko/pull/336)
* Extract filesystem in order rather than in reverse [#326](https://github.com/GoogleContainerTools/kaniko/pull/326)
* Configure logs to show colors [#327](https://github.com/GoogleContainerTools/kaniko/pull/327)
* Enable shared config for s3 [#321](https://github.com/GoogleContainerTools/kaniko/pull/321)
* Update go-containerregistry. [#305](https://github.com/GoogleContainerTools/kaniko/pull/305)
* Tag latest in cloudbuild.yaml [#287](https://github.com/GoogleContainerTools/kaniko/pull/287)
* Set default home value [#281](https://github.com/GoogleContainerTools/kaniko/pull/281)
* Update deps [#265](https://github.com/GoogleContainerTools/kaniko/pull/265)
* Update go-containerregistry dep and remove unnecessary Options [#376](https://github.com/GoogleContainerTools/kaniko/pull/376)
* Add a bit more context to layer offset failures [#264](https://github.com/GoogleContainerTools/kaniko/pull/264)

## Bug Fixes
* Whitelist /busybox in the debug image [#369](https://github.com/GoogleContainerTools/kaniko/pull/369)
* Check --cache-repo is provided with --cache and --no-push [#374](https://github.com/GoogleContainerTools/kaniko/pull/374)
* Fixes a whitelist issue when untarring files in ADD commands. [#371](https://github.com/GoogleContainerTools/kaniko/pull/371)
* set default HOME env properly [#341](https://github.com/GoogleContainerTools/kaniko/pull/341)
* Review config for cmd/entrypoint after building a stage [#348](https://github.com/GoogleContainerTools/kaniko/pull/348)
* Enable overwriting of links (solves #351) [#360](https://github.com/GoogleContainerTools/kaniko/pull/360)
* Only return stdout when running commands for integration tests [#363](https://github.com/GoogleContainerTools/kaniko/pull/363)
* Whitelist /etc/mtab [#347](https://github.com/GoogleContainerTools/kaniko/pull/347)
* Added a KanikoStage type for each stage of a Dockerfile [#320](https://github.com/GoogleContainerTools/kaniko/pull/320)
* Make sure paths are absolute before matching files to wildcard sources [#330](https://github.com/GoogleContainerTools/kaniko/pull/330)
* Build each kaniko image separately [#324](https://github.com/GoogleContainerTools/kaniko/pull/324)
* support multiple tags when writing to a tarfile [#323](https://github.com/GoogleContainerTools/kaniko/pull/323)
* Snapshot only specific files for COPY [#319](https://github.com/GoogleContainerTools/kaniko/pull/319)
* Remove some constraints from our Gopkg.toml. [#318](https://github.com/GoogleContainerTools/kaniko/pull/318)
* Always snapshot files in COPY and RUN commands [#289](https://github.com/GoogleContainerTools/kaniko/pull/289)
* Refactor command line arguments and the executor [#306](https://github.com/GoogleContainerTools/kaniko/pull/306)
* Fix bug in SaveStage function for multistage builds [#295](https://github.com/GoogleContainerTools/kaniko/pull/295)
* Get absolute path of file before checking whitelist [#293](https://github.com/GoogleContainerTools/kaniko/pull/293)
* Fix support for insecure registry [#169](https://github.com/GoogleContainerTools/kaniko/pull/169)
* ignore sockets when adding to tar [#288](https://github.com/GoogleContainerTools/kaniko/pull/288)
* fix add command bug when adding remote URLs [#277](https://github.com/GoogleContainerTools/kaniko/pull/277)
* Environment variables with multiple '=' are not parsed correctly [#278](https://github.com/GoogleContainerTools/kaniko/pull/278)
* Ensure cmd.SysProcAttr is set before modifying it [#275](https://github.com/GoogleContainerTools/kaniko/pull/275)
* Don't copy same files twice in copy integration tests [#273](https://github.com/GoogleContainerTools/kaniko/pull/273)
* Extract intermediate stages to filesystem [#266](https://github.com/GoogleContainerTools/kaniko/pull/266)
* Fix process group handling. [#271](https://github.com/GoogleContainerTools/kaniko/pull/271)
* Only add whiteout files once [#270](https://github.com/GoogleContainerTools/kaniko/pull/270)
* Fix handling of the volume directive [#334](https://github.com/GoogleContainerTools/kaniko/pull/334)


# v0.3.0 Release - 2018-07-31
New Features
* Local integration testing [#256](https://github.com/GoogleContainerTools/kaniko/pull/256)
* Add --target flag for multistage builds [#255](https://github.com/GoogleContainerTools/kaniko/pull/255)
* Look for on cluster credentials using k8s chain [#243](https://github.com/GoogleContainerTools/kaniko/pull/243)

Bug Fixes
* Kill grandchildren spun up by child processes [#247](https://github.com/GoogleContainerTools/kaniko/issues/247)
* Fix bug in copy command [#221](https://github.com/GoogleContainerTools/kaniko/issues/221)
* Multi-stage errors when referencing earlier stages [#233](https://github.com/GoogleContainerTools/kaniko/issues/233)


# v0.2.0 Release - 2018-07-09

New Features
* Support for adding different source contexts, including Amazon S3 [#195](https://github.com/GoogleContainerTools/kaniko/issues/195)
* Added --reproducible [#205](https://github.com/GoogleContainerTools/kaniko/pull/205) and --single-snapshot [#204](https://github.com/GoogleContainerTools/kaniko/pull/204) flags
* Documented running kaniko in gVisor [#194](https://github.com/GoogleContainerTools/kaniko/pull/194)
* Update go-containerregistry so kaniko works better with Harbor and Gitlab[#227](https://github.com/GoogleContainerTools/kaniko/pull/227)
* Push image to multiple destinations [#184](https://github.com/GoogleContainerTools/kaniko/pull/184)

# v0.1.0 Release - 2018-05-17

New Features
* The majority of Dockerfile commands are feature complete [#1](https://github.com/GoogleContainerTools/kaniko/issues/1)
* Support for multi-stage Dockerfile builds [#141](https://github.com/GoogleContainerTools/kaniko/pull/141)
* Refactored integration tests [#126](https://github.com/GoogleContainerTools/kaniko/pull/126)
* Added debug image with a busybox shell [#171](https://github.com/GoogleContainerTools/kaniko/pull/1710)
* Added credential helper for Amazon ECR [#167](https://github.com/GoogleContainerTools/kaniko/pull/167)
 
