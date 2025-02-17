PORTNAME=	kak-lsp
DISTVERSIONPREFIX=	v
DISTVERSION=	14.1.0
PORTREVISION=	3
CATEGORIES=	editors

MAINTAINER=	mikael@FreeBSD.org
COMMENT=	Kakoune Language Server Protocol Client
WWW=		https://github.com/ul/kak-lsp

LICENSE=	UNLICENSE
LICENSE_FILE=	${WRKSRC}/UNLICENSE

RUN_DEPENDS=	kakoune>=2018.10.27:editors/kakoune

USES=		cargo
USE_GITHUB=	yes
GH_ACCOUNT=	ul

CARGO_CRATES=	adler32-1.2.0 \
		aho-corasick-0.7.19 \
		arc-swap-1.5.1 \
		atty-0.2.14 \
		autocfg-1.1.0 \
		bitflags-1.3.2 \
		boxfnonce-0.1.1 \
		bumpalo-3.4.0 \
		cfg-if-0.1.10 \
		cfg-if-1.0.0 \
		chrono-0.4.20 \
		clap-3.2.20 \
		clap_lex-0.2.4 \
		crc32fast-1.3.2 \
		crossbeam-channel-0.5.6 \
		crossbeam-utils-0.8.11 \
		daemonize-0.4.1 \
		diffs-0.4.1 \
		dirs-2.0.2 \
		dirs-next-2.0.0 \
		dirs-sys-0.3.7 \
		dirs-sys-next-0.1.2 \
		either-1.8.0 \
		enum_primitive-0.1.1 \
		field-offset-0.3.4 \
		form_urlencoded-1.0.1 \
		futures-0.3.24 \
		futures-channel-0.3.24 \
		futures-core-0.3.24 \
		futures-executor-0.3.24 \
		futures-io-0.3.24 \
		futures-macro-0.3.24 \
		futures-sink-0.3.24 \
		futures-task-0.3.24 \
		futures-util-0.3.24 \
		getopts-0.2.21 \
		getrandom-0.2.7 \
		glob-0.3.0 \
		hashbrown-0.12.3 \
		hermit-abi-0.1.19 \
		idna-0.2.3 \
		indexmap-1.9.1 \
		indoc-1.0.7 \
		itertools-0.10.3 \
		itoa-1.0.3 \
		js-sys-0.3.55 \
		jsonrpc-core-18.0.0 \
		lazy_static-1.4.0 \
		libc-0.2.132 \
		libflate-1.2.0 \
		libflate_lz77-1.1.0 \
		log-0.4.17 \
		lsp-types-0.93.2 \
		matches-0.1.9 \
		memchr-2.5.0 \
		memoffset-0.6.5 \
		num-integer-0.1.45 \
		num-traits-0.1.43 \
		num-traits-0.2.15 \
		num_threads-0.1.6 \
		once_cell-1.14.0 \
		os_str_bytes-6.3.0 \
		percent-encoding-2.1.0 \
		pest-2.3.0 \
		pin-project-lite-0.2.9 \
		pin-utils-0.1.0 \
		ppv-lite86-0.2.16 \
		proc-macro2-1.0.43 \
		pulldown-cmark-0.9.2 \
		quote-1.0.21 \
		rand-0.8.5 \
		rand_chacha-0.3.1 \
		rand_core-0.6.3 \
		redox_syscall-0.2.16 \
		redox_users-0.4.3 \
		regex-1.6.0 \
		regex-syntax-0.6.27 \
		rle-decode-fast-1.0.3 \
		ropey-1.5.0 \
		rustc_version-0.3.3 \
		rustversion-1.0.9 \
		ryu-1.0.11 \
		semver-0.11.0 \
		semver-parser-0.10.2 \
		serde-1.0.144 \
		serde_derive-1.0.144 \
		serde_json-1.0.85 \
		serde_repr-0.1.9 \
		slab-0.4.7 \
		slog-2.7.0 \
		slog-async-2.7.0 \
		slog-kvfilter-0.7.0 \
		slog-scope-4.4.0 \
		slog-stdlog-4.1.1 \
		slog-term-2.9.0 \
		sloggers-2.1.1 \
		smallvec-1.9.0 \
		str_indices-0.4.0 \
		strsim-0.10.0 \
		syn-1.0.99 \
		take_mut-0.2.2 \
		term-0.7.0 \
		termcolor-1.1.3 \
		textwrap-0.15.0 \
		thiserror-1.0.34 \
		thiserror-impl-1.0.34 \
		thread_local-1.1.4 \
		time-0.1.44 \
		time-0.3.14 \
		time-macros-0.2.4 \
		tinyvec-1.6.0 \
		tinyvec_macros-0.1.0 \
		toml-0.5.9 \
		trackable-1.2.0 \
		trackable_derive-1.0.0 \
		ucd-trie-0.1.5 \
		unicase-2.6.0 \
		unicode-bidi-0.3.8 \
		unicode-ident-1.0.3 \
		unicode-normalization-0.1.21 \
		unicode-width-0.1.9 \
		unindent-0.1.10 \
		url-2.2.2 \
		version_check-0.9.4 \
		wasi-0.10.0+wasi-snapshot-preview1 \
		wasi-0.11.0+wasi-snapshot-preview1 \
		wasm-bindgen-0.2.78 \
		wasm-bindgen-backend-0.2.78 \
		wasm-bindgen-macro-0.2.78 \
		wasm-bindgen-macro-support-0.2.78 \
		wasm-bindgen-shared-0.2.78 \
		web-sys-0.3.55 \
		whoami-1.2.2 \
		widestring-0.4.3 \
		winapi-0.3.9 \
		winapi-i686-pc-windows-gnu-0.4.0 \
		winapi-util-0.1.5 \
		winapi-x86_64-pc-windows-gnu-0.4.0 \
		windows-acl-0.3.0

SUB_FILES=	pkg-message

PLIST_FILES=	bin/kak-lsp \
		"@sample ${ETCDIR}/kak-lsp.toml.sample"
PORTDOCS=	README.asciidoc

OPTIONS_DEFINE=	DOCS

post-install:
	${STRIP_CMD} ${STAGEDIR}${PREFIX}/bin/kak-lsp
	@${MKDIR} ${STAGEDIR}${ETCDIR}
	${INSTALL_DATA} ${WRKSRC}/kak-lsp.toml ${STAGEDIR}${ETCDIR}/kak-lsp.toml.sample

post-install-DOCS-on:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/README.asciidoc ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>
