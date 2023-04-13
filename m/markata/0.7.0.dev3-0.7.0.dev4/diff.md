# Comparing `tmp/markata-0.7.0.dev3.tar.gz` & `tmp/markata-0.7.0.dev4.tar.gz`

## Comparing `markata-0.7.0.dev3.tar` & `markata-0.7.0.dev4.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.markataignore
--rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/CHANGELOG.md
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/contributing.md
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata.toml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/10cd58be07625a78
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/12ca7ce6efec36dc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/1436ccdb7f623e24
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/1b6d0dc8bfe07f44
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/326d8b79bff4520a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/33045a6d4d2ea649
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/3cd919ed06211bdc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/461ac3e4828f6373
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/46a3e79b61b953b1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/46a6e9f7cb71c400
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/484d33d30ad6f03b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/4866e4b89f378d09
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/4de1ad9c5a2a6c70
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/501c9fb7b755da93
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/5cc374fba8ee541e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/5f689cea3fce3bb1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/5f7e18d7cae18b2c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/61f7d44b0ab14a09
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/69b56a5830c2197b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/6acadf45c462e52d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/6bbcc74f059357bb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/70645821045181fc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/79cf11143dede548
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/7c167d9ee572478d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/81d2eaf080de8506
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/8848185bf6aa4e3b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/89c873ee97dbb039
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/8b449b92cfeac07c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/9463176557607f8f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/967120ab24403222
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/9a254f816eebaa36
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/9f0dda6bb1383981
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/a6cf756c570cf407
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/a937f467a79a88cd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/adf046d1ea0fde5d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/af9acc35038f9ad1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/b508b4f54eedabd3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/b5a6784b28f77fb4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/b9c537991bfeacd9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/bb82eeacc57ed21f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/bd6afaa6f3c789e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/c0598e39b88c9587
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/c07b51aed7c60564
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/c78c06618c910d01
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/d28aac70dfaef279
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/d7564ace8a02b553
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/e79b6a4b5892a423
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/ecc22e34af12e78
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/ee285978c650d124
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/faf00fa823ccd1dc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/fc820843b951895b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/fd73eadd970ac148
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/ff03871d25af7de3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.ruff_cache/content/fff32de9536317a4
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/404.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/color-theme.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/home-page.md
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/index.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/nav.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/project-gallery/markata_dev.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/docs/project-gallery/waylonwalker.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/__about__.py
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/__main__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/background.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/errors.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/hookspec.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/lifecycle.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/standard_config.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/__main__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/cli.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/header.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/plugins.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/runner.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/server.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/cli/summary.py
--rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/Karla-Regular.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/auto_description.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/auto_title.py
--rw-r--r--   0        0        0    16607 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/base_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/copy_assets.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/covers.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/create_covers.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/datetime.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/default_doc_template.md
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/default_log_template.html
--rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/default_post_template.html
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/default_redirect_template.html
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/default_service_worker_template.js
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/docs.py
--rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/feeds.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/flat_slug.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/generator.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/glob.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/heading_link.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/icon_resize.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/jinja_md.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/load.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/manifest.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/md_it_highlight_code.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/md_it_wikilinks.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/mdit_details.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/post_template.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/prevnext.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/prevnext_template.html
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/publish_dev_to_source.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/publish_html.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/publish_source.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/pyinstrument.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/redirects.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/render_markdown.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/rss.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/seo.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/service_worker.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/setup_logging.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/sitemap.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/subroute.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/to_json.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/plugins/tui.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/markata/scripts/migrate_to_slugify.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/_redirects
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/favicon.ico
--rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/markata.dev_.webp
--rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/markata.dev_markata_plugins_base-cli_.webp
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/robots.txt
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/waylonwalker.com.webp
--rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/waylonwalker.com_archive.webp
--rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/static/waylonwalker.com_markata-configure-head.webp
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/test_doc_page.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/test_feeds.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/test_one_default_page.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/test_one_default_page_with_path_prefix.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/plugins/conftest.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/plugins/test_default_post_template.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/plugins/test_flat_slug.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/tests/plugins/test_redirects.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/LICENSE
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/README.md
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 markata-0.7.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.markataignore
+-rw-r--r--   0        0        0    17178 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/CHANGELOG.md
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/contributing.md
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata.toml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/180e5a108f3ccbe7
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/1a070b1c9d232bd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/25bf8629a87794a5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/263e8e879d18ebac
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/27b69d6c8bb27e98
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/4463da003e1d5d6d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/4ddfe90d5a081bf2
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/55de486a97ed5b45
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/598113e8307bad3b
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/5bb9eb5de75dcb48
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/5e5545ed2a075cfa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/605ba62e77fc5ec6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/606f7454f4cb95be
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/61da2feb0344f2cb
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/6a27d81a591b70ef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/6a58bb1b9ee8dfbe
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/6b320b2cc847a860
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/7633a2671ad6f45f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/77c24ef6a2fa0b67
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/862985b3483d35a9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/92ed4cc05e0b9ce8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/94650a2d4244d7cf
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/a5721cf41597b162
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/a612715f33343b31
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/aeef740d124251e3
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/b9092fe9367ffb1d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/baff6231fec68b23
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/bdd7eccf9b145655
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/bf9859d9d526cf14
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/c09ffa07ba16a806
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/c29d8de91d64cc36
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/c68ab9a3316f656a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/c7aee0c5afaec710
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/c80266dbdec69eef
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/ced607beb20e77d8
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/d17dce40fb98f481
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/d4a2a4cc12e20b5e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/d52320af7ace676a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/d7e341f9b09a3fd6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/d9c44fe8f08555fe
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/de5a059a35a2b644
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/e15b656953b5be51
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/e18ecf0770d8d4d5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/e32d1f7d56ebbd04
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/e709a5da3d694cb9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/ea8076bd8ad2498
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/eb2fb6dcbfd99e4f
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/ee5251c09a9428ed
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f05669e2921ebb60
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f272f16ecde8a0c6
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f699eae0889307b5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f73bd8d450980be9
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f94f902c7ffbb04d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.ruff_cache/content/f9b3b8b2e64ecd9
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/404.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/color-theme.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/home-page.md
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/index.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/nav.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/project-gallery/markata_dev.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/docs/project-gallery/waylonwalker.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/__about__.py
+-rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/__main__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/background.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/errors.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/hookspec.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/lifecycle.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/standard_config.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/__main__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/cli.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/header.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/plugins.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/runner.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/server.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/cli/summary.py
+-rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/Karla-Regular.ttf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/auto_description.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/auto_title.py
+-rw-r--r--   0        0        0    16607 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/base_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/copy_assets.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/covers.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/create_covers.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/datetime.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/default_doc_template.md
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/default_log_template.html
+-rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/default_post_template.html
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/default_redirect_template.html
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/default_service_worker_template.js
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/docs.py
+-rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/feeds.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/flat_slug.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/generator.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/glob.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/heading_link.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/icon_resize.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/jinja_md.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/load.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/manifest.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/md_it_highlight_code.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/md_it_wikilinks.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/mdit_details.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/post_template.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/prevnext.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/prevnext_template.html
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/publish_dev_to_source.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/publish_html.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/publish_source.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/pyinstrument.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/redirects.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/render_markdown.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/rss.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/seo.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/service_worker.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/setup_logging.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/sitemap.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/subroute.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/to_json.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/plugins/tui.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/markata/scripts/migrate_to_slugify.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/_redirects
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/favicon.ico
+-rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/markata.dev_.webp
+-rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/markata.dev_markata_plugins_base-cli_.webp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/robots.txt
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/waylonwalker.com.webp
+-rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/waylonwalker.com_archive.webp
+-rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/static/waylonwalker.com_markata-configure-head.webp
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/test_doc_page.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/test_feeds.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/test_one_default_page.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/test_one_default_page_with_path_prefix.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/plugins/test_default_post_template.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/plugins/test_flat_slug.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/tests/plugins/test_redirects.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/LICENSE
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/README.md
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 markata-0.7.0.dev4/PKG-INFO
```

### Comparing `markata-0.7.0.dev3/CHANGELOG.md` & `markata-0.7.0.dev4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/CODE_OF_CONDUCT.md` & `markata-0.7.0.dev4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/contributing.md` & `markata-0.7.0.dev4/contributing.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata.toml` & `markata-0.7.0.dev4/markata.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/color-theme.md` & `markata-0.7.0.dev4/docs/color-theme.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/home-page.md` & `markata-0.7.0.dev4/docs/home-page.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/index.md` & `markata-0.7.0.dev4/docs/index.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/nav.md` & `markata-0.7.0.dev4/docs/nav.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/project-gallery/markata_dev.md` & `markata-0.7.0.dev4/docs/project-gallery/markata_dev.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/docs/project-gallery/waylonwalker.md` & `markata-0.7.0.dev4/docs/project-gallery/waylonwalker.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/__init__.py` & `markata-0.7.0.dev4/markata/__init__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/background.py` & `markata-0.7.0.dev4/markata/background.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/hookspec.py` & `markata-0.7.0.dev4/markata/hookspec.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/lifecycle.py` & `markata-0.7.0.dev4/markata/lifecycle.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/standard_config.py` & `markata-0.7.0.dev4/markata/standard_config.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/__main__.py` & `markata-0.7.0.dev4/markata/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/cli.py` & `markata-0.7.0.dev4/markata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/plugins.py` & `markata-0.7.0.dev4/markata/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/runner.py` & `markata-0.7.0.dev4/markata/cli/runner.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/server.py` & `markata-0.7.0.dev4/markata/cli/server.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/cli/summary.py` & `markata-0.7.0.dev4/markata/cli/summary.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/Karla-Regular.ttf` & `markata-0.7.0.dev4/markata/plugins/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/auto_description.py` & `markata-0.7.0.dev4/markata/plugins/auto_description.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/base_cli.py` & `markata-0.7.0.dev4/markata/plugins/base_cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/copy_assets.py` & `markata-0.7.0.dev4/markata/plugins/copy_assets.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/covers.py` & `markata-0.7.0.dev4/markata/plugins/covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/create_covers.py` & `markata-0.7.0.dev4/markata/plugins/create_covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/datetime.py` & `markata-0.7.0.dev4/markata/plugins/datetime.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/default_doc_template.md` & `markata-0.7.0.dev4/markata/plugins/default_doc_template.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/default_log_template.html` & `markata-0.7.0.dev4/markata/plugins/default_log_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/default_post_template.html` & `markata-0.7.0.dev4/markata/plugins/default_post_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/default_redirect_template.html` & `markata-0.7.0.dev4/markata/plugins/default_redirect_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/default_service_worker_template.js` & `markata-0.7.0.dev4/markata/plugins/default_service_worker_template.js`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/docs.py` & `markata-0.7.0.dev4/markata/plugins/docs.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/feeds.py` & `markata-0.7.0.dev4/markata/plugins/feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/flat_slug.py` & `markata-0.7.0.dev4/markata/plugins/flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/generator.py` & `markata-0.7.0.dev4/markata/plugins/generator.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/glob.py` & `markata-0.7.0.dev4/markata/plugins/glob.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/heading_link.py` & `markata-0.7.0.dev4/markata/plugins/heading_link.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/icon_resize.py` & `markata-0.7.0.dev4/markata/plugins/icon_resize.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/jinja_md.py` & `markata-0.7.0.dev4/markata/plugins/jinja_md.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/load.py` & `markata-0.7.0.dev4/markata/plugins/load.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/manifest.py` & `markata-0.7.0.dev4/markata/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/md_it_highlight_code.py` & `markata-0.7.0.dev4/markata/plugins/md_it_highlight_code.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/md_it_wikilinks.py` & `markata-0.7.0.dev4/markata/plugins/md_it_wikilinks.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/mdit_details.py` & `markata-0.7.0.dev4/markata/plugins/mdit_details.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/post_template.py` & `markata-0.7.0.dev4/markata/plugins/post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/prevnext.py` & `markata-0.7.0.dev4/markata/plugins/prevnext.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/prevnext_template.html` & `markata-0.7.0.dev4/markata/plugins/prevnext_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/publish_dev_to_source.py` & `markata-0.7.0.dev4/markata/plugins/publish_dev_to_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/publish_html.py` & `markata-0.7.0.dev4/markata/plugins/publish_html.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/publish_source.py` & `markata-0.7.0.dev4/markata/plugins/publish_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/pyinstrument.py` & `markata-0.7.0.dev4/markata/plugins/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/redirects.py` & `markata-0.7.0.dev4/markata/plugins/redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/render_markdown.py` & `markata-0.7.0.dev4/markata/plugins/render_markdown.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/rss.py` & `markata-0.7.0.dev4/markata/plugins/rss.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/seo.py` & `markata-0.7.0.dev4/markata/plugins/seo.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/service_worker.py` & `markata-0.7.0.dev4/markata/plugins/service_worker.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/setup_logging.py` & `markata-0.7.0.dev4/markata/plugins/setup_logging.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/sitemap.py` & `markata-0.7.0.dev4/markata/plugins/sitemap.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/subroute.py` & `markata-0.7.0.dev4/markata/plugins/subroute.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/plugins/tui.py` & `markata-0.7.0.dev4/markata/plugins/tui.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/markata/scripts/migrate_to_slugify.py` & `markata-0.7.0.dev4/markata/scripts/migrate_to_slugify.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/_redirects` & `markata-0.7.0.dev4/static/_redirects`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/favicon.ico` & `markata-0.7.0.dev4/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/markata.dev_.webp` & `markata-0.7.0.dev4/static/markata.dev_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/markata.dev_markata_plugins_base-cli_.webp` & `markata-0.7.0.dev4/static/markata.dev_markata_plugins_base-cli_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/waylonwalker.com.webp` & `markata-0.7.0.dev4/static/waylonwalker.com.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/waylonwalker.com_archive.webp` & `markata-0.7.0.dev4/static/waylonwalker.com_archive.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/static/waylonwalker.com_markata-configure-head.webp` & `markata-0.7.0.dev4/static/waylonwalker.com_markata-configure-head.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/test_doc_page.py` & `markata-0.7.0.dev4/tests/test_doc_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/test_feeds.py` & `markata-0.7.0.dev4/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/test_one_default_page.py` & `markata-0.7.0.dev4/tests/test_one_default_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/test_one_default_page_with_path_prefix.py` & `markata-0.7.0.dev4/tests/test_one_default_page_with_path_prefix.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/plugins/test_default_post_template.py` & `markata-0.7.0.dev4/tests/plugins/test_default_post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/plugins/test_flat_slug.py` & `markata-0.7.0.dev4/tests/plugins/test_flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/tests/plugins/test_redirects.py` & `markata-0.7.0.dev4/tests/plugins/test_redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/.gitignore` & `markata-0.7.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/LICENSE` & `markata-0.7.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/README.md` & `markata-0.7.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.0.dev3/pyproject.toml` & `markata-0.7.0.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
  "checksumdir",
  "cookiecutter",
  "copier",
  "deepmerge",
  "diskcache",
  "feedgen",
  "jinja2",
+ "linkify-it-py",
  "markdown-it-py[plugins]",
  "markdown2[all]",
  "more-itertools",
  "pathspec",
  "pillow",
  "pluggy",
  "pymdown-extensions",
```

### Comparing `markata-0.7.0.dev3/PKG-INFO` & `markata-0.7.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markata
-Version: 0.7.0.dev3
+Version: 0.7.0.dev4
 Summary: Static site generator plugins all the way down.
 Project-URL: Homepage, https://markata.dev
 Project-URL: Changelog, https://markata.dev/CHANGELOG/
 Project-URL: Source, https://github.com/waylonwalker/markata
 Project-URL: Issues, https://github.com/waylonwalker/markata/issues
 Project-URL: Documentation, https://markata.dev
 Author-email: Waylon Walker <waylon@waylonwalker.com>, waylon@markata.dev
@@ -56,14 +56,15 @@
 Requires-Dist: checksumdir
 Requires-Dist: cookiecutter
 Requires-Dist: copier
 Requires-Dist: deepmerge
 Requires-Dist: diskcache
 Requires-Dist: feedgen
 Requires-Dist: jinja2
+Requires-Dist: linkify-it-py
 Requires-Dist: markdown-it-py[plugins]
 Requires-Dist: markdown2[all]
 Requires-Dist: more-itertools
 Requires-Dist: pathspec
 Requires-Dist: pillow
 Requires-Dist: pluggy
 Requires-Dist: pymdown-extensions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: markata Version: 0.7.0.dev3 Summary: Static site
+Metadata-Version: 2.1 Name: markata Version: 0.7.0.dev4 Summary: Static site
 generator plugins all the way down. Project-URL: Homepage, https://markata.dev
 Project-URL: Changelog, https://markata.dev/CHANGELOG/ Project-URL: Source,
 https://github.com/waylonwalker/markata Project-URL: Issues, https://
 github.com/waylonwalker/markata/issues Project-URL: Documentation, https://
 markata.dev Author-email: Waylon Walker
 waylonwalker.com>, waylon@markata.dev License: Copyright (c) 2012-2022 Waylon
 Walker Permission is hereby granted, free of charge, to any person obtaining a
@@ -30,27 +30,27 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
 Language :: Python :: Implementation :: PyPy Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development Classifier: Topic :: Text Processing
 Classifier: Typing :: Typed Requires-Python: >=3.6 Requires-Dist: anyconfig
 Requires-Dist: beautifulsoup4 Requires-Dist: checksumdir Requires-Dist:
 cookiecutter Requires-Dist: copier Requires-Dist: deepmerge Requires-Dist:
-diskcache Requires-Dist: feedgen Requires-Dist: jinja2 Requires-Dist: markdown-
-it-py[plugins] Requires-Dist: markdown2[all] Requires-Dist: more-itertools
-Requires-Dist: pathspec Requires-Dist: pillow Requires-Dist: pluggy Requires-
-Dist: pymdown-extensions Requires-Dist: python-frontmatter Requires-Dist:
-python-slugify Requires-Dist: pytz Requires-Dist: rich Requires-Dist:
-textual<0.2.0 Requires-Dist: toml Requires-Dist: typer Provides-Extra: dev
-Requires-Dist: black; extra == 'dev' Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: interrogate; extra == 'dev' Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: pytest-mock; extra ==
-'dev' Requires-Dist: pytest-tmp-files; extra == 'dev' Requires-Dist: ruff;
-extra == 'dev' Provides-Extra: pyinstrument Requires-Dist: pyinstrument; extra
-== 'pyinstrument' Description-Content-Type: text/markdown
+diskcache Requires-Dist: feedgen Requires-Dist: jinja2 Requires-Dist: linkify-
+it-py Requires-Dist: markdown-it-py[plugins] Requires-Dist: markdown2[all]
+Requires-Dist: more-itertools Requires-Dist: pathspec Requires-Dist: pillow
+Requires-Dist: pluggy Requires-Dist: pymdown-extensions Requires-Dist: python-
+frontmatter Requires-Dist: python-slugify Requires-Dist: pytz Requires-Dist:
+rich Requires-Dist: textual<0.2.0 Requires-Dist: toml Requires-Dist: typer
+Provides-Extra: dev Requires-Dist: black; extra == 'dev' Requires-Dist: hatch;
+extra == 'dev' Requires-Dist: interrogate; extra == 'dev' Requires-Dist: mypy;
+extra == 'dev' Requires-Dist: pre-commit; extra == 'dev' Requires-Dist: pytest;
+extra == 'dev' Requires-Dist: pytest-cov; extra == 'dev' Requires-Dist: pytest-
+mock; extra == 'dev' Requires-Dist: pytest-tmp-files; extra == 'dev' Requires-
+Dist: ruff; extra == 'dev' Provides-Extra: pyinstrument Requires-Dist:
+pyinstrument; extra == 'pyinstrument' Description-Content-Type: text/markdown
                                     ******
                                [Markata] ******
                   Markdown to site, plugins all the way down
 A static site generator that will give you a great site with many standard web
 features like rss, sitemaps, and seo tags, out of the box. Running `markata
 build` will get you a that only requires you to write Markdown. If you have
 additional features that you want, don't worry, since markata is built
```

