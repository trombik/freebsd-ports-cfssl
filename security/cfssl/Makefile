# Created by: Yuri Victorovich <yuri@rawbw.com>

PORTNAME=	cfssl
DISTVERSION=	1.6.1
CATEGORIES=	security
MASTER_SITES=	https://bitbucket.org/${GOOSE_ACCOUNT}/${GOOSE_PROJECT}/get/${GOOSE_COMMIT}.tar.gz?dummy=goose-${GOOSE_COMMIT}.tar.gz/:goose
DISTFILES=	goose-${GOOSE_COMMIT}.tar.gz:goose

MAINTAINER=	yuri@rawbw.com
COMMENT=	CloudFlares PKI and TLS toolkit

LICENSE=	BSD2CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

LIB_DEPENDS=	libltdl.so:devel/libltdl

USES=	go:no_targets gmake
USE_GITHUB=	yes
GH_ACCOUNT= cloudflare
GH_TAGNAME=	v${DISTVERSION}

GH_TUPLE=	\
	GeertJohan:go.incremental:v1.0.0:geertjohan_go_incremental/vendor/github.com/GeertJohan/go.incremental \
	GeertJohan:go.rice:v1.0.2:geertjohan_go_rice/vendor/github.com/GeertJohan/go.rice \
	akavel:rsrc:v0.8.0:akavel_rsrc/vendor/github.com/akavel/rsrc \
	beorn7:perks:v1.0.1:beorn7_perks/vendor/github.com/beorn7/perks \
	bgentry:speakeasy:v0.1.0:bgentry_speakeasy/vendor/github.com/bgentry/speakeasy \
	census-instrumentation:opencensus-proto:v0.3.0:census_instrumentation_opencensus_proto/vendor/github.com/census-instrumentation/opencensus-proto \
	certifi:gocertifi:431795d63e8d:certifi_gocertifi/vendor/github.com/certifi/gocertifi \
	cespare:xxhash:v2.1.1:cespare_xxhash/vendor/github.com/cespare/xxhash/v2 \
	cheggaaa:pb:v1.0.28:cheggaaa_pb/vendor/gopkg.in/cheggaaa/pb.v1 \
	cloudflare:backoff:647f3cdfc87a:cloudflare_backoff/vendor/github.com/cloudflare/backoff \
	cloudflare:redoctober:99c99a8e7544:cloudflare_redoctober/vendor/github.com/cloudflare/redoctober \
	cncf:udpa:6414d713912e:cncf_udpa/vendor/github.com/cncf/udpa/go \
	coreos:go-semver:v0.3.0:coreos_go_semver/vendor/github.com/coreos/go-semver \
	coreos:go-systemd:v22.3.2:coreos_go_systemd/vendor/github.com/coreos/go-systemd/v22 \
	cpuguy83:go-md2man:v2.0.0:cpuguy83_go_md2man/vendor/github.com/cpuguy83/go-md2man/v2 \
	daaku:go.zipexe:v1.0.1:daaku_go_zipexe/vendor/github.com/daaku/go.zipexe \
	davecgh:go-spew:v1.1.1:davecgh_go_spew/vendor/github.com/davecgh/go-spew \
	dominikh:go-tools:v0.1.4:dominikh_go_tools/vendor/honnef.co/go/tools \
	dustin:go-humanize:v1.0.0:dustin_go_humanize/vendor/github.com/dustin/go-humanize \
	envoyproxy:go-control-plane:668b12f5399d:envoyproxy_go_control_plane/vendor/github.com/envoyproxy/go-control-plane \
	envoyproxy:protoc-gen-validate:v0.6.1:envoyproxy_protoc_gen_validate/vendor/github.com/envoyproxy/protoc-gen-validate \
	etcd-io:bbolt:v1.3.5:etcd_io_bbolt/vendor/go.etcd.io/bbolt \
	form3tech-oss:jwt-go:v3.2.3:form3tech_oss_jwt_go/vendor/github.com/form3tech-oss/jwt-go \
	fullstorydev:grpcurl:v1.8.1:fullstorydev_grpcurl/vendor/github.com/fullstorydev/grpcurl \
	getsentry:raven-go:v0.2.0:getsentry_raven_go/vendor/github.com/getsentry/raven-go \
	go-sql-driver:mysql:v1.6.0:go_sql_driver_mysql/vendor/github.com/go-sql-driver/mysql \
	go-yaml:yaml:496545a6307b:go_yaml_yaml/vendor/gopkg.in/yaml.v3 \
	go-yaml:yaml:v2.4.0:go_yaml_yaml_1/vendor/gopkg.in/yaml.v2 \
	gogo:protobuf:v1.3.2:gogo_protobuf/vendor/github.com/gogo/protobuf \
	golang:appengine:v1.6.7:golang_appengine/vendor/google.golang.org/appengine \
	golang:crypto:38f3c27a63bf:golang_crypto/vendor/golang.org/x/crypto \
	golang:glog:424d2337a529:golang_glog/vendor/github.com/golang/glog \
	golang:groupcache:41bb18bfe9da:golang_groupcache/vendor/github.com/golang/groupcache \
	golang:lint:6edffad5e616:golang_lint/vendor/golang.org/x/lint \
	golang:mock:v1.5.0:golang_mock/vendor/github.com/golang/mock \
	golang:mod:v0.4.2:golang_mod/vendor/golang.org/x/mod \
	golang:net:4163338589ed:golang_net/vendor/golang.org/x/net \
	golang:oauth2:81ed05c6b58c:golang_oauth2/vendor/golang.org/x/oauth2 \
	golang:protobuf:v1.5.2:golang_protobuf/vendor/github.com/golang/protobuf \
	golang:sys:b0526f3d8744:golang_sys/vendor/golang.org/x/sys \
	golang:text:v0.3.6:golang_text/vendor/golang.org/x/text \
	golang:time:f8bda1e9f3ba:golang_time/vendor/golang.org/x/time \
	golang:tools:v0.1.0:golang_tools/vendor/golang.org/x/tools \
	golang:xerrors:5ec99f83aff1:golang_xerrors/vendor/golang.org/x/xerrors \
	google:btree:v1.0.1:google_btree/vendor/github.com/google/btree \
	google:certificate-transparency-go:373a877eec92:google_certificate_transparency_go/vendor/github.com/google/certificate-transparency-go \
	google:go-cmp:v0.5.5:google_go_cmp/vendor/github.com/google/go-cmp \
	google:go-genproto:fb37daa5cd7a:google_go_genproto/vendor/google.golang.org/genproto \
	google:uuid:v1.2.0:google_uuid/vendor/github.com/google/uuid \
	googleapis:google-cloud-go:v0.81.0:googleapis_google_cloud_go/vendor/cloud.google.com/go \
	gorilla:websocket:v1.4.2:gorilla_websocket/vendor/github.com/gorilla/websocket \
	grpc-ecosystem:go-grpc-middleware:v1.3.0:grpc_ecosystem_go_grpc_middleware/vendor/github.com/grpc-ecosystem/go-grpc-middleware \
	grpc-ecosystem:go-grpc-prometheus:v1.2.0:grpc_ecosystem_go_grpc_prometheus/vendor/github.com/grpc-ecosystem/go-grpc-prometheus \
	grpc-ecosystem:grpc-gateway:v1.16.0:grpc_ecosystem_grpc_gateway/vendor/github.com/grpc-ecosystem/grpc-gateway \
	grpc:grpc-go:v1.37.0:grpc_grpc_go/vendor/google.golang.org/grpc \
	inconshreveable:mousetrap:v1.0.0:inconshreveable_mousetrap/vendor/github.com/inconshreveable/mousetrap \
	jessevdk:go-flags:v1.4.0:jessevdk_go_flags/vendor/github.com/jessevdk/go-flags \
	jhump:protoreflect:v1.8.2:jhump_protoreflect/vendor/github.com/jhump/protoreflect \
	jmhodges:clock:880ee4c33548:jmhodges_clock/vendor/github.com/jmhodges/clock \
	jmoiron:sqlx:v1.3.3:jmoiron_sqlx/vendor/github.com/jmoiron/sqlx \
	jonboulle:clockwork:v0.2.2:jonboulle_clockwork/vendor/github.com/jonboulle/clockwork \
	json-iterator:go:v1.1.11:json_iterator_go/vendor/github.com/json-iterator/go \
	kisielk:sqlstruct:5f3e10d3ab46:kisielk_sqlstruct/vendor/github.com/kisielk/sqlstruct \
	kisom:goutils:v1.4.3:kisom_goutils/vendor/github.com/kisom/goutils \
	kubernetes-sigs:yaml:v1.2.0:kubernetes_sigs_yaml/vendor/sigs.k8s.io/yaml \
	kylelemons:go-gypsy:v1.0.0:kylelemons_go_gypsy/vendor/github.com/kylelemons/go-gypsy \
	lib:pq:v1.10.1:lib_pq/vendor/github.com/lib/pq \
	mattn:go-runewidth:v0.0.12:mattn_go_runewidth/vendor/github.com/mattn/go-runewidth \
	mattn:go-sqlite3:v1.14.7:mattn_go_sqlite3/vendor/github.com/mattn/go-sqlite3 \
	matttproud:golang_protobuf_extensions:v1.0.1:matttproud_golang_protobuf_extensions/vendor/github.com/matttproud/golang_protobuf_extensions \
	modern-go:concurrent:bacd9c7ef1dd:modern_go_concurrent/vendor/github.com/modern-go/concurrent \
	modern-go:reflect2:v1.0.1:modern_go_reflect2/vendor/github.com/modern-go/reflect2 \
	nkovacs:streamquote:v1.0.0:nkovacs_streamquote/vendor/github.com/nkovacs/streamquote \
	olekukonko:tablewriter:v0.0.5:olekukonko_tablewriter/vendor/github.com/olekukonko/tablewriter \
	pkg:errors:v0.9.1:pkg_errors/vendor/github.com/pkg/errors \
	pmezard:go-difflib:v1.0.0:pmezard_go_difflib/vendor/github.com/pmezard/go-difflib \
	prometheus:client_golang:v1.10.0:prometheus_client_golang/vendor/github.com/prometheus/client_golang \
	prometheus:client_model:v0.2.0:prometheus_client_model/vendor/github.com/prometheus/client_model \
	prometheus:common:v0.24.0:prometheus_common/vendor/github.com/prometheus/common \
	prometheus:procfs:v0.6.0:prometheus_procfs/vendor/github.com/prometheus/procfs \
	rivo:uniseg:v0.2.0:rivo_uniseg/vendor/github.com/rivo/uniseg \
	russross:blackfriday:v2.1.0:russross_blackfriday/vendor/github.com/russross/blackfriday/v2 \
	sirupsen:logrus:v1.8.1:sirupsen_logrus/vendor/github.com/sirupsen/logrus \
	soheilhy:cmux:v0.1.5:soheilhy_cmux/vendor/github.com/soheilhy/cmux \
	spf13:cobra:v1.1.3:spf13_cobra/vendor/github.com/spf13/cobra \
	spf13:pflag:v1.0.5:spf13_pflag/vendor/github.com/spf13/pflag \
	stretchr:testify:v1.7.0:stretchr_testify/vendor/github.com/stretchr/testify \
	tmc:grpc-websocket-proxy:e5319fda7802:tmc_grpc_websocket_proxy/vendor/github.com/tmc/grpc-websocket-proxy \
	uber-go:atomic:v1.7.0:uber_go_atomic/vendor/go.uber.org/atomic \
	uber-go:multierr:v1.7.0:uber_go_multierr/vendor/go.uber.org/multierr \
	uber-go:zap:v1.16.0:uber_go_zap/vendor/go.uber.org/zap \
	urfave:cli:v1.22.5:urfave_cli/vendor/github.com/urfave/cli \
	valyala:bytebufferpool:v1.0.0:valyala_bytebufferpool/vendor/github.com/valyala/bytebufferpool \
	valyala:fasttemplate:v1.0.1:valyala_fasttemplate/vendor/github.com/valyala/fasttemplate \
	weppos:publicsuffix-go:b1f36a2d6c0b:weppos_publicsuffix_go/vendor/github.com/weppos/publicsuffix-go \
	xiang90:probing:43a291ad63a2:xiang90_probing/vendor/github.com/xiang90/probing \
	ziutek:mymysql:v1.5.4:ziutek_mymysql/vendor/github.com/ziutek/mymysql \
	zmap:zcrypto:18f1e0152cfc:zmap_zcrypto/vendor/github.com/zmap/zcrypto \
	zmap:zlint:v3.1.0:zmap_zlint/vendor/github.com/zmap/zlint/v3

	# Mirrors for the following packages are not currently known, please look them up and handle these tuples manually:
	#	::8488cc47d90c:group_name/vendor/bitbucket.org/liamstask/goose
	#	::v1.26.0:group_name/vendor/google.golang.org/protobuf
	#	::v2.305.0-alpha.0:group_name/vendor/go.etcd.io/etcd/client/v2
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/api/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/client/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/etcdctl/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/pkg/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/raft/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/server/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/tests/v3
	#	::v3.5.0-alpha.0:group_name/vendor/go.etcd.io/etcd/v3

CFSSL_GH_TUPLE=	\
	protocolbuffers:protobuf-go:v1.26.0:protocolbuffers_protobuf_go/vendor/google.golang.org/protobuf \
	etcd-io:etcd:v2.305.0-alpha.0:group_name/vendor/go.etcd.io/etcd/client/v2 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/api/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/client/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/etcdctl/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/pkg/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/raft/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/server/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/tests/v3 \
	etcd-io:etcd:v3.5.0-alpha.0:etcd_io_etcd/vendor/go.etcd.io/etcd/v3 \
GH_TUPLE+=	${CFSSL_GH_TUPLE} \

# XXX for unresolable goose
GOOSE_ACCOUNT=	liamstask
GOOSE_PROJECT=	goose
GOOSE_COMMIT=	8488cc47d90c

pre-configure:
	${REINPLACE_CMD} -e 's|%%DISTVERSION%%|${DISTVERSION}|g' ${WRKSRC}/cli/version/version.go

# the project uses Makefile for build and installation
do-build:
	(cd ${WRKSRC} && \
	${SETENV} ${MAKE_ENV} ${GO_ENV} ${MAKE_CMD} ${MAKE_FLAGS} ${MAKEFILE} ${_MAKE_JOBS} all)

do-install:
	# XXX define GOBIN
	# Makefile is used but the install target uses go install.
	(cd ${WRKSRC} && \
	${SETENV} ${MAKE_ENV} ${GO_ENV} GOBIN=${STAGEDIR}${PREFIX}/bin ${MAKE_CMD} ${MAKE_FLAGS} ${MAKEFILE} ${_MAKE_JOBS} install)
.for F in cfssl cfssl-certinfo multirootca
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/${F}
.endfor

.include <bsd.port.mk>
