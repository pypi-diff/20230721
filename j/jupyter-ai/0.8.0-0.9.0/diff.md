# Comparing `tmp/jupyter_ai-0.8.0.tar.gz` & `tmp/jupyter_ai-0.9.0.tar.gz`

## Comparing `jupyter_ai-0.8.0.tar` & `jupyter_ai-0.9.0.tar`

### file list

```diff
@@ -1,163 +1,160 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.eslintignore
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/babel.config.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jest.config.js
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/_version.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/engine.py
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/extension.py
--rw-r--r--   0        0        0    11226 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/models.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/reply_processor.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/task_manager.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tasks.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/__init__.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/ask.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/base.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/chat_provider.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/config.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/default.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/embeddings_provider.py
--rw-r--r--   0        0        0     9042 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/generate.py
--rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/learn.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/memory.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/providers.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/actors/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4486 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
--rw-r--r--   0        0        0    26351 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/253.0b5d158f3577d0bfbee5.js
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
--rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
--rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
--rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/643.ca949b2ea9d252cbcc23.js
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js
--rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
--rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
--rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js.LICENSE.txt
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
--rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
--rw-r--r--   0        0        0    11319 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/remoteEntry.e77e7c805bbe3d26eec6.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/schema/plugin.json
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/chat_handler.ts
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/icons.ts
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/index.ts
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/inserter.ts
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/selection-watcher.ts
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/__tests__/widgets/closable-dialog.spec.tsx
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-messages.tsx
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/open-task-dialog.tsx
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/select.tsx
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/components/settings/model-fields.tsx
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/types/svg.d.ts
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/src/widgets/closable-dialog.tsx
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/base.css
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/chat-settings.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/index.js
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/icons/chat.svg
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/LICENSE
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/README.md
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 jupyter_ai-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.eslintignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/babel.config.js
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jest.config.js
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/engine.py
+-rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/models.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/reply_processor.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/task_manager.py
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tasks.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/__init__.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/ask.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/base.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/chat_provider.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/config.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/default.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/embeddings_provider.py
+-rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/generate.py
+-rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/learn.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/memory.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/providers.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/actors/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf
+-rw-r--r--   0        0        0    26382 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/253.4cb04dcfead6f07b8e7c.js
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff
+-rw-r--r--   0        0        0    41113 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js.LICENSE.txt
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js
+-rw-r--r--   0        0        0   157509 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js.LICENSE.txt
+-rw-r--r--   0        0        0  1568438 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js.LICENSE.txt
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/643.23e0a9c561346f879c77.js
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js
+-rw-r--r--   0        0        0     9772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff
+-rw-r--r--   0        0        0   443772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js.LICENSE.txt
+-rw-r--r--   0        0        0    91736 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js.LICENSE.txt
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff
+-rw-r--r--   0        0        0   272943 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf
+-rw-r--r--   0        0        0    11315 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/remoteEntry.9095dd2e94ae47ffc04b.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   111460 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/schema/plugin.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/chat_handler.ts
+-rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/icons.ts
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/index.ts
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/inserter.ts
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/theme-provider.ts
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/select.tsx
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/components/settings/model-fields.tsx
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/base.css
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/chat-settings.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/index.js
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/icons/chat.svg
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/README.md
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 jupyter_ai-0.9.0/PKG-INFO
```

### Comparing `jupyter_ai-0.8.0/.eslintrc.js` & `jupyter_ai-0.9.0/.eslintrc.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,15 @@
         'eslint:recommended',
         'plugin:@typescript-eslint/eslint-recommended',
         'plugin:@typescript-eslint/recommended',
         'plugin:prettier/recommended'
     ],
     parser: '@typescript-eslint/parser',
     parserOptions: {
+        tsconfigRootDir: __dirname,
         project: './tsconfig.json'
     },
     plugins: ['@typescript-eslint'],
     rules: {
         '@typescript-eslint/naming-convention': [
             'error', {
                 selector: 'interface',
@@ -34,11 +35,11 @@
                 allowTemplateLiterals: false
             }
         ],
         curly: ['error', 'all'],
         eqeqeq: 'error',
         'prefer-arrow-callback': 'error'
     },
-    overrides: {
+    overrides: [{
         files: ['src/**/*']
-    }
+    }]
 };
```

### Comparing `jupyter_ai-0.8.0/RELEASE.md` & `jupyter_ai-0.9.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jest.config.js` & `jupyter_ai-0.9.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/package.json` & `jupyter_ai-0.9.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745192307692306%*

 * *Differences: {"'scripts'": '{\'dev-install\': \'pip install -e ".[dev,all]" && jupyter labextension develop . '*

 * *              "--overwrite && jupyter server extension enable jupyter_ai'}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -97,15 +97,15 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
+        "dev-install": "pip install -e \".[dev,all]\" && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
         "dev-uninstall": "pip uninstall jupyter_ai -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyter_ai-0.8.0/tsconfig.json` & `jupyter_ai-0.9.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/__init__.py` & `jupyter_ai-0.9.0/jupyter_ai/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from ._version import __version__
-from .extension import AiExtension
-
 # expose jupyter_ai_magics ipython extension
 from jupyter_ai_magics import load_ipython_extension, unload_ipython_extension
 
+from ._version import __version__
+
 # imports to expose entry points. DO NOT REMOVE.
 from .engine import GPT3ModelEngine
-from .tasks import tasks
+from .extension import AiExtension
 
 # imports to expose types to other AI modules. DO NOT REMOVE.
-from .tasks import DefaultTaskDefinition
+from .tasks import DefaultTaskDefinition, tasks
+
 
 def _jupyter_labextension_paths():
-    return [{
-        "src": "labextension",
-        "dest": "@jupyter-ai/core"
-    }]
+    return [{"src": "labextension", "dest": "@jupyter-ai/core"}]
+
 
 def _jupyter_server_extension_points():
-    return [{
-        "module": "jupyter_ai",
-        "app": AiExtension
-    }]
+    return [{"module": "jupyter_ai", "app": AiExtension}]
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/engine.py` & `jupyter_ai-0.9.0/jupyter_ai/engine.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,58 @@
-from abc import abstractmethod, ABC, ABCMeta
+from abc import ABC, ABCMeta, abstractmethod
 from typing import Dict
+
 import openai
 from traitlets.config import LoggingConfigurable, Unicode
+
 from .task_manager import DescribeTaskResponse
 
+
 class BaseModelEngineMetaclass(ABCMeta, type(LoggingConfigurable)):
     pass
 
+
 class BaseModelEngine(ABC, LoggingConfigurable, metaclass=BaseModelEngineMetaclass):
     id: str
     name: str
 
     # these two attributes are currently reserved but unused.
     input_type: str
     output_type: str
-  
+
     @abstractmethod
-    async def execute(self, task: DescribeTaskResponse, prompt_variables: Dict[str, str]):
+    async def execute(
+        self, task: DescribeTaskResponse, prompt_variables: Dict[str, str]
+    ):
         pass
 
+
 class GPT3ModelEngine(BaseModelEngine):
     id = "gpt3"
     name = "GPT-3"
-    modalities = [
-        "txt2txt"
-    ]
-
-    api_key = Unicode(
-        config=True,
-        help="OpenAI API key",
-        allow_none=False
-    )
+    modalities = ["txt2txt"]
+
+    api_key = Unicode(config=True, help="OpenAI API key", allow_none=False)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    async def execute(self, task: DescribeTaskResponse, prompt_variables: Dict[str, str]):
+    async def execute(
+        self, task: DescribeTaskResponse, prompt_variables: Dict[str, str]
+    ):
         if "body" not in prompt_variables:
             raise Exception("Prompt body must be specified.")
 
         prompt = task.prompt_template.format(**prompt_variables)
         self.log.info(f"GPT3 prompt:\n{prompt}")
-        
+
         openai.api_key = self.api_key
         response = await openai.Completion.acreate(
             model="text-davinci-003",
             prompt=prompt,
             temperature=0.7,
             max_tokens=256,
             top_p=1,
             frequency_penalty=0,
-            presence_penalty=0
+            presence_penalty=0,
         )
-        return response['choices'][0]['text']
+        return response["choices"][0]["text"]
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/extension.py` & `jupyter_ai-0.9.0/jupyter_ai/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,40 @@
 import asyncio
+import inspect
 
+import ray
+from importlib_metadata import entry_points
+from jupyter_ai.actors.ask import AskActor
+from jupyter_ai.actors.base import ACTOR_TYPE
 from jupyter_ai.actors.chat_provider import ChatProviderActor
 from jupyter_ai.actors.config import ConfigActor
+from jupyter_ai.actors.default import DefaultActor
 from jupyter_ai.actors.embeddings_provider import EmbeddingsProviderActor
-from jupyter_ai.actors.providers import ProvidersActor
-
-from jupyter_ai_magics.utils import load_providers
-
-from langchain.memory import ConversationBufferWindowMemory
-from jupyter_ai.actors.default import DefaultActor 
-from jupyter_ai.actors.ask import AskActor 
+from jupyter_ai.actors.generate import GenerateActor
 from jupyter_ai.actors.learn import LearnActor
-from jupyter_ai.actors.router import Router
 from jupyter_ai.actors.memory import MemoryActor
-from jupyter_ai.actors.generate import GenerateActor
-from jupyter_ai.actors.base import ACTOR_TYPE
+from jupyter_ai.actors.providers import ProvidersActor
+from jupyter_ai.actors.router import Router
 from jupyter_ai.reply_processor import ReplyProcessor
+from jupyter_ai_magics.utils import load_providers
 from jupyter_server.extension.application import ExtensionApp
+from langchain.memory import ConversationBufferWindowMemory
+from ray.util.queue import Queue
 
+from .engine import BaseModelEngine
 from .handlers import (
-    ChatHandler, 
-    ChatHistoryHandler, 
-    EmbeddingsModelProviderHandler, 
-    ModelProviderHandler, 
-    PromptAPIHandler, 
+    ChatHandler,
+    ChatHistoryHandler,
+    EmbeddingsModelProviderHandler,
+    GlobalConfigHandler,
+    ModelProviderHandler,
+    PromptAPIHandler,
     TaskAPIHandler,
-    GlobalConfigHandler
 )
 
-from importlib_metadata import entry_points
-import inspect
-from .engine import BaseModelEngine
-
-import ray
-from ray.util.queue import Queue
-from jupyter_ai_magics.utils import load_providers
-
 
 class AiExtension(ExtensionApp):
     name = "jupyter_ai"
     handlers = [
         ("api/ai/config", GlobalConfigHandler),
         ("api/ai/prompt", PromptAPIHandler),
         (r"api/ai/tasks/?", TaskAPIHandler),
@@ -47,140 +42,156 @@
         (r"api/ai/chats/?", ChatHandler),
         (r"api/ai/chats/history?", ChatHistoryHandler),
         (r"api/ai/providers?", ModelProviderHandler),
         (r"api/ai/providers/embeddings?", EmbeddingsModelProviderHandler),
     ]
 
     @property
-    def ai_engines(self): 
+    def ai_engines(self):
         if "ai_engines" not in self.settings:
             self.settings["ai_engines"] = {}
 
         return self.settings["ai_engines"]
-    
 
     def initialize_settings(self):
         ray.init()
 
         # EP := entry point
         eps = entry_points()
-        
+
         ## step 1: instantiate model engines and bind them to settings
         model_engine_class_eps = eps.select(group="jupyter_ai.model_engine_classes")
-        
+
         if not model_engine_class_eps:
-            self.log.error("No model engines found for jupyter_ai.model_engine_classes group. One or more model engines are required for AI extension to work.")
+            self.log.error(
+                "No model engines found for jupyter_ai.model_engine_classes group. One or more model engines are required for AI extension to work."
+            )
             return
 
         for model_engine_class_ep in model_engine_class_eps:
             try:
                 Engine = model_engine_class_ep.load()
             except:
-                self.log.error(f"Unable to load model engine class from entry point `{model_engine_class_ep.name}`.")
+                self.log.error(
+                    f"Unable to load model engine class from entry point `{model_engine_class_ep.name}`."
+                )
                 continue
 
             if not inspect.isclass(Engine) or not issubclass(Engine, BaseModelEngine):
-                self.log.error(f"Unable to instantiate model engine class from entry point `{model_engine_class_ep.name}` as it is not a subclass of `BaseModelEngine`.")
+                self.log.error(
+                    f"Unable to instantiate model engine class from entry point `{model_engine_class_ep.name}` as it is not a subclass of `BaseModelEngine`."
+                )
                 continue
 
             try:
                 self.ai_engines[Engine.id] = Engine(config=self.config, log=self.log)
             except:
-                self.log.error(f"Unable to instantiate model engine class from entry point `{model_engine_class_ep.name}`.")
+                self.log.error(
+                    f"Unable to instantiate model engine class from entry point `{model_engine_class_ep.name}`."
+                )
                 continue
 
             self.log.info(f"Registered engine `{Engine.id}`.")
 
         ## step 2: load default tasks and bind them to settings
         module_default_tasks_eps = eps.select(group="jupyter_ai.default_tasks")
 
         if not module_default_tasks_eps:
             self.settings["ai_default_tasks"] = []
             return
-        
+
         default_tasks = []
         for module_default_tasks_ep in module_default_tasks_eps:
             try:
                 module_default_tasks = module_default_tasks_ep.load()
             except:
-                self.log.error(f"Unable to load task from entry point `{module_default_tasks_ep.name}`")
+                self.log.error(
+                    f"Unable to load task from entry point `{module_default_tasks_ep.name}`"
+                )
                 continue
-            
+
             default_tasks += module_default_tasks
 
         self.settings["ai_default_tasks"] = default_tasks
         self.log.info("Registered all default tasks.")
 
         providers = load_providers(log=self.log)
         self.settings["chat_providers"] = providers
         self.log.info("Registered providers.")
 
         self.log.info(f"Registered {self.name} server extension")
 
         # Store chat clients in a dictionary
         self.settings["chat_clients"] = {}
         self.settings["chat_handlers"] = {}
-        
+
         # store chat messages in memory for now
         # this is only used to render the UI, and is not the conversational
         # memory object used by the LM chain.
         self.settings["chat_history"] = []
 
-
         reply_queue = Queue()
         self.settings["reply_queue"] = reply_queue
 
         router = Router.options(name=ACTOR_TYPE.ROUTER).remote(
             reply_queue=reply_queue,
             log=self.log,
         )
         default_actor = DefaultActor.options(name=ACTOR_TYPE.DEFAULT.value).remote(
-            reply_queue=reply_queue, 
+            reply_queue=reply_queue,
             log=self.log,
-            chat_history=self.settings["chat_history"]
+            chat_history=self.settings["chat_history"],
         )
 
-        providers_actor = ProvidersActor.options(name=ACTOR_TYPE.PROVIDERS.value).remote(
+        providers_actor = ProvidersActor.options(
+            name=ACTOR_TYPE.PROVIDERS.value
+        ).remote(
             log=self.log,
         )
         config_actor = ConfigActor.options(name=ACTOR_TYPE.CONFIG.value).remote(
             log=self.log,
         )
-        chat_provider_actor = ChatProviderActor.options(name=ACTOR_TYPE.CHAT_PROVIDER.value).remote(
+        chat_provider_actor = ChatProviderActor.options(
+            name=ACTOR_TYPE.CHAT_PROVIDER.value
+        ).remote(
             log=self.log,
         )
-        embeddings_provider_actor = EmbeddingsProviderActor.options(name=ACTOR_TYPE.EMBEDDINGS_PROVIDER.value).remote(
+        embeddings_provider_actor = EmbeddingsProviderActor.options(
+            name=ACTOR_TYPE.EMBEDDINGS_PROVIDER.value
+        ).remote(
             log=self.log,
         )
         learn_actor = LearnActor.options(name=ACTOR_TYPE.LEARN.value).remote(
             reply_queue=reply_queue,
             log=self.log,
             root_dir=self.serverapp.root_dir,
         )
         ask_actor = AskActor.options(name=ACTOR_TYPE.ASK.value).remote(
-            reply_queue=reply_queue, 
+            reply_queue=reply_queue,
             log=self.log,
         )
         memory_actor = MemoryActor.options(name=ACTOR_TYPE.MEMORY.value).remote(
             log=self.log,
             memory=ConversationBufferWindowMemory(return_messages=True, k=2),
         )
         generate_actor = GenerateActor.options(name=ACTOR_TYPE.GENERATE.value).remote(
-            reply_queue=reply_queue, 
+            reply_queue=reply_queue,
             log=self.log,
-            root_dir=self.settings['server_root_dir'],
+            root_dir=self.settings["server_root_dir"],
         )
-     
-        self.settings['router'] = router
-        self.settings['providers_actor'] = providers_actor
-        self.settings['config_actor'] = config_actor
-        self.settings['chat_provider_actor'] = chat_provider_actor
-        self.settings['embeddings_provider_actor'] = embeddings_provider_actor
+
+        self.settings["router"] = router
+        self.settings["providers_actor"] = providers_actor
+        self.settings["config_actor"] = config_actor
+        self.settings["chat_provider_actor"] = chat_provider_actor
+        self.settings["embeddings_provider_actor"] = embeddings_provider_actor
         self.settings["default_actor"] = default_actor
         self.settings["learn_actor"] = learn_actor
         self.settings["ask_actor"] = ask_actor
         self.settings["memory_actor"] = memory_actor
         self.settings["generate_actor"] = generate_actor
 
-        reply_processor = ReplyProcessor(self.settings['chat_handlers'], reply_queue, log=self.log)        
+        reply_processor = ReplyProcessor(
+            self.settings["chat_handlers"], reply_queue, log=self.log
+        )
         loop = asyncio.get_event_loop()
-        loop.create_task(reply_processor.start())            
+        loop.create_task(reply_processor.start())
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/handlers.py` & `jupyter_ai-0.9.0/jupyter_ai/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-from dataclasses import asdict
+import getpass
 import json
+import time
+import uuid
+from dataclasses import asdict
 from typing import Dict, List
-from jupyter_ai.actors.base import ACTOR_TYPE
+
 import ray
 import tornado
-import uuid
-import time
-import getpass
-
-from tornado.web import HTTPError
+from jupyter_ai.actors.base import ACTOR_TYPE
+from jupyter_server.base.handlers import APIHandler as BaseAPIHandler
+from jupyter_server.base.handlers import JupyterHandler
+from jupyter_server.utils import ensure_async
 from pydantic import ValidationError
-
 from tornado import web, websocket
-
-from jupyter_server.base.handlers import APIHandler as BaseAPIHandler, JupyterHandler
-from jupyter_server.utils import ensure_async
-
-from .task_manager import TaskManager
+from tornado.web import HTTPError
 
 from .models import (
-    ChatHistory,
-    ChatUser, 
-    ListProvidersEntry, 
-    ListProvidersResponse, 
-    PromptRequest, 
-    ChatRequest, 
-    ChatMessage, 
-    Message, 
-    AgentChatMessage, 
-    HumanChatMessage, 
-    ConnectionMessage, 
+    AgentChatMessage,
     ChatClient,
-    GlobalConfig
+    ChatHistory,
+    ChatMessage,
+    ChatRequest,
+    ChatUser,
+    ConnectionMessage,
+    GlobalConfig,
+    HumanChatMessage,
+    ListProvidersEntry,
+    ListProvidersResponse,
+    Message,
+    PromptRequest,
 )
+from .task_manager import TaskManager
 
 
 class APIHandler(BaseAPIHandler):
     @property
-    def engines(self): 
+    def engines(self):
         return self.settings["ai_engines"]
-    
+
     @property
     def default_tasks(self):
         return self.settings["ai_default_tasks"]
 
     @property
     def task_manager(self):
         # we have to create the TaskManager lazily, since no event loop is
         # running in ServerApp.initialize_settings().
         if "task_manager" not in self.settings:
-            self.settings["task_manager"] = TaskManager(engines=self.engines, default_tasks=self.default_tasks)
+            self.settings["task_manager"] = TaskManager(
+                engines=self.engines, default_tasks=self.default_tasks
+            )
         return self.settings["task_manager"]
-    
+
+
 class PromptAPIHandler(APIHandler):
     @tornado.web.authenticated
     async def post(self):
         try:
             request = PromptRequest(**self.get_json_body())
         except ValidationError as e:
             self.log.exception(e)
@@ -64,70 +65,67 @@
         if request.engine_id not in self.engines:
             raise HTTPError(500, f"Model engine not registered: {request.engine_id}")
 
         engine = self.engines[request.engine_id]
         task = await self.task_manager.describe_task(request.task_id)
         if not task:
             raise HTTPError(404, f"Task not found with ID: {request.task_id}")
-        
+
         output = await ensure_async(engine.execute(task, request.prompt_variables))
 
-        self.finish(json.dumps({
-            "output": output,
-            "insertion_mode": task.insertion_mode
-        }))
+        self.finish(
+            json.dumps({"output": output, "insertion_mode": task.insertion_mode})
+        )
+
 
 class TaskAPIHandler(APIHandler):
     @tornado.web.authenticated
     async def get(self, id=None):
         if id is None:
             list_tasks_response = await self.task_manager.list_tasks()
             self.finish(json.dumps(list_tasks_response.dict()))
             return
-        
+
         describe_task_response = await self.task_manager.describe_task(id)
         if describe_task_response is None:
             raise HTTPError(404, f"Task not found with ID: {id}")
 
         self.finish(json.dumps(describe_task_response.dict()))
 
 
 class ChatHistoryHandler(BaseAPIHandler):
     """Handler to return message history"""
 
     _messages = []
-    
+
     @property
     def chat_history(self):
         return self.settings["chat_history"]
-    
+
     @chat_history.setter
     def _chat_history_setter(self, new_history):
         self.settings["chat_history"] = new_history
-    
+
     @tornado.web.authenticated
     async def get(self):
         history = ChatHistory(messages=self.chat_history)
         self.finish(history.json())
 
 
-class ChatHandler(
-    JupyterHandler,
-    websocket.WebSocketHandler
-):
+class ChatHandler(JupyterHandler, websocket.WebSocketHandler):
     """
     A websocket handler for chat.
     """
-    
+
     @property
-    def chat_handlers(self) -> Dict[str, 'ChatHandler']:
+    def chat_handlers(self) -> Dict[str, "ChatHandler"]:
         """Dictionary mapping client IDs to their WebSocket handler
         instances."""
         return self.settings["chat_handlers"]
-    
+
     @property
     def chat_clients(self) -> Dict[str, ChatClient]:
         """Dictionary mapping client IDs to their ChatClient objects that store
         metadata."""
         return self.settings["chat_clients"]
 
     @property
@@ -139,16 +137,15 @@
     def chat_history(self) -> List[ChatMessage]:
         return self.settings["chat_history"]
 
     def initialize(self):
         self.log.debug("Initializing websocket connection %s", self.request.path)
 
     def pre_get(self):
-        """Handles authentication/authorization.
-        """
+        """Handles authentication/authorization."""
         # authenticate the request before opening the websocket
         user = self.current_user
         if user is None:
             self.log.warning("Couldn't authenticate WebSocket connection")
             raise web.HTTPError(403)
 
         # authorize the user.
@@ -164,27 +161,25 @@
     def get_chat_user(self) -> ChatUser:
         """Retrieves the current user. If collaborative mode is disabled, one
         is synthesized from the login."""
         collaborative = self.config.get("LabApp", {}).get("collaborative", False)
 
         if collaborative:
             return ChatUser(**asdict(self.current_user))
-        
-        
+
         login = getpass.getuser()
         return ChatUser(
             username=login,
             initials=login[0].capitalize(),
             name=login,
             display_name=login,
             color=None,
-            avatar_url=None
+            avatar_url=None,
         )
 
-
     def generate_client_id(self):
         """Generates a client ID to identify the current WS connection."""
         return uuid.uuid4().hex
 
     def open(self):
         """Handles opening of a WebSocket connection. Client ID can be retrieved
         from `self.client_id`."""
@@ -197,33 +192,35 @@
         self.client_id = client_id
         self.write_message(ConnectionMessage(client_id=client_id).dict())
 
         self.log.info(f"Client connected. ID: {client_id}")
         self.log.debug("Clients are : %s", self.chat_handlers.keys())
 
     def broadcast_message(self, message: Message):
-        """Broadcasts message to all connected clients. 
+        """Broadcasts message to all connected clients.
         Appends message to `self.chat_history`.
         """
 
         self.log.debug("Broadcasting message: %s to all clients...", message)
         client_ids = self.chat_handlers.keys()
-        
+
         for client_id in client_ids:
             client = self.chat_handlers[client_id]
             if client:
                 client.write_message(message.dict())
-        
+
         # Only append ChatMessage instances to history, not control messages
-        if isinstance(message, HumanChatMessage) or isinstance(message, AgentChatMessage):
+        if isinstance(message, HumanChatMessage) or isinstance(
+            message, AgentChatMessage
+        ):
             self.chat_history.append(message)
 
     async def on_message(self, message):
         self.log.debug("Message recieved: %s", message)
-        
+
         try:
             message = json.loads(message)
             chat_request = ChatRequest(**message)
         except ValidationError as e:
             self.log.error(e)
             return
 
@@ -236,17 +233,17 @@
             client=self.chat_client,
         )
 
         # broadcast the message to other clients
         self.broadcast_message(message=chat_message)
 
         # Clear the message history if given the /clear command
-        if chat_request.prompt.startswith('/'):
-            command = chat_request.prompt.split(' ', 1)[0]
-            if command == '/clear':
+        if chat_request.prompt.startswith("/"):
+            command = chat_request.prompt.split(" ", 1)[0]
+            if command == "/clear":
                 self.chat_history.clear()
 
         # process through the router
         router = ray.get_actor("router")
         router.process_message.remote(chat_message)
 
     def on_close(self):
@@ -257,19 +254,19 @@
 
         self.log.info(f"Client disconnected. ID: {self.client_id}")
         self.log.debug("Chat clients: %s", self.chat_handlers.keys())
 
 
 class ModelProviderHandler(BaseAPIHandler):
     @property
-    def chat_providers(self): 
+    def chat_providers(self):
         actor = ray.get_actor("providers")
         o = actor.get_model_providers.remote()
         return ray.get(o)
-    
+
     @web.authenticated
     def get(self):
         providers = []
         for provider in self.chat_providers.values():
             # skip old legacy OpenAI chat provider used only in magics
             if provider.id == "openai-chat":
                 continue
@@ -280,21 +277,22 @@
                     name=provider.name,
                     models=provider.models,
                     auth_strategy=provider.auth_strategy,
                     registry=provider.registry,
                     fields=provider.fields,
                 )
             )
-        
-        response = ListProvidersResponse(providers=sorted(providers, key=lambda p: p.name))
+
+        response = ListProvidersResponse(
+            providers=sorted(providers, key=lambda p: p.name)
+        )
         self.finish(response.json())
 
 
 class EmbeddingsModelProviderHandler(BaseAPIHandler):
-    
     @property
     def embeddings_providers(self):
         actor = ray.get_actor("providers")
         o = actor.get_embeddings_providers.remote()
         return ray.get(o)
 
     @web.authenticated
@@ -307,31 +305,33 @@
                     name=provider.name,
                     models=provider.models,
                     auth_strategy=provider.auth_strategy,
                     registry=provider.registry,
                     fields=provider.fields,
                 )
             )
-        
-        response = ListProvidersResponse(providers=sorted(providers, key=lambda p: p.name))
+
+        response = ListProvidersResponse(
+            providers=sorted(providers, key=lambda p: p.name)
+        )
         self.finish(response.json())
 
 
 class GlobalConfigHandler(BaseAPIHandler):
     """API handler for fetching and setting the
     model and emebddings config.
     """
-    
+
     @web.authenticated
     def get(self):
         actor = ray.get_actor(ACTOR_TYPE.CONFIG)
         config = ray.get(actor.get_config.remote())
         if not config:
             raise HTTPError(500, "No config found.")
-        
+
         self.finish(config.json())
 
     @web.authenticated
     def post(self):
         try:
             config = GlobalConfig(**self.get_json_body())
             actor = ray.get_actor(ACTOR_TYPE.CONFIG)
@@ -341,14 +341,13 @@
             self.finish()
 
         except ValidationError as e:
             self.log.exception(e)
             raise HTTPError(500, str(e)) from e
         except ValueError as e:
             self.log.exception(e)
-            raise HTTPError(500, str(e.cause) if hasattr(e, 'cause') else str(e))
+            raise HTTPError(500, str(e.cause) if hasattr(e, "cause") else str(e))
         except Exception as e:
             self.log.exception(e)
             raise HTTPError(
                 500, "Unexpected error occurred while updating the config."
             ) from e
-
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/models.py` & `jupyter_ai-0.9.0/jupyter_ai/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,113 +1,127 @@
+from typing import Any, Dict, List, Literal, Optional, Union
+
 from jupyter_ai_magics.providers import AuthStrategy, Field
+from pydantic import BaseModel
 
-from pydantic import BaseModel 
-from typing import Any, Dict, List, Union, Literal, Optional
 
 class PromptRequest(BaseModel):
     task_id: str
     engine_id: str
     prompt_variables: Dict[str, str]
 
+
 # the type of message used to chat with the agent
 class ChatRequest(BaseModel):
     prompt: str
 
+
 class ChatUser(BaseModel):
     # User ID assigned by IdentityProvider.
     username: str
     initials: str
     name: str
     display_name: str
     color: Optional[str]
     avatar_url: Optional[str]
 
+
 class ChatClient(ChatUser):
     # A unique client ID assigned to identify different JupyterLab clients on
     # the same device (i.e. running on multiple tabs/windows), which may have
     # the same username assigned to them by the IdentityProvider.
     id: str
 
+
 class AgentChatMessage(BaseModel):
     type: Literal["agent"] = "agent"
     id: str
     time: float
     body: str
     # message ID of the HumanChatMessage it is replying to
     reply_to: str
 
+
 class HumanChatMessage(BaseModel):
     type: Literal["human"] = "human"
     id: str
     time: float
     body: str
     client: ChatClient
 
+
 class ConnectionMessage(BaseModel):
     type: Literal["connection"] = "connection"
     client_id: str
 
+
 class ClearMessage(BaseModel):
     type: Literal["clear"] = "clear"
 
+
 # the type of messages being broadcast to clients
 ChatMessage = Union[
     AgentChatMessage,
     HumanChatMessage,
 ]
 
-Message = Union[
-    AgentChatMessage,
-    HumanChatMessage,
-    ConnectionMessage,
-    ClearMessage
-]
+Message = Union[AgentChatMessage, HumanChatMessage, ConnectionMessage, ClearMessage]
+
 
 class ListEnginesEntry(BaseModel):
     id: str
     name: str
 
+
 class ListTasksEntry(BaseModel):
     id: str
     name: str
 
+
 class ListTasksResponse(BaseModel):
     tasks: List[ListTasksEntry]
 
+
 class DescribeTaskResponse(BaseModel):
     name: str
     insertion_mode: str
     prompt_template: str
     engines: List[ListEnginesEntry]
 
+
 class ChatHistory(BaseModel):
     """History of chat messages"""
+
     messages: List[ChatMessage]
 
 
 class ListProvidersEntry(BaseModel):
     """Model provider with supported models
     and provider's authentication strategy
     """
+
     id: str
     name: str
     models: List[str]
     auth_strategy: AuthStrategy
     registry: bool
     fields: List[Field]
 
 
 class ListProvidersResponse(BaseModel):
     providers: List[ListProvidersEntry]
 
+
 class IndexedDir(BaseModel):
     path: str
 
+
 class IndexMetadata(BaseModel):
     dirs: List[IndexedDir]
 
+
 class GlobalConfig(BaseModel):
     model_provider_id: Optional[str] = None
     embeddings_provider_id: Optional[str] = None
     api_keys: Dict[str, str] = {}
     send_with_shift_enter: Optional[bool] = None
     fields: Dict[str, Dict[str, Any]] = {}
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/reply_processor.py` & `jupyter_ai-0.9.0/jupyter_ai/reply_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import asyncio
 from typing import Dict
+
 from jupyter_ai.handlers import ChatHandler
 from ray.util.queue import Queue
 
 
-class ReplyProcessor():
+class ReplyProcessor:
     """A single processor to distribute replies"""
 
     def __init__(self, handlers: Dict[str, ChatHandler], queue: Queue, log):
         self.handlers = handlers
         self.queue = queue
         self.log = log
 
     def process(self, message):
-        self.log.debug('Processing message %s in ReplyProcessor', message)
+        self.log.debug("Processing message %s in ReplyProcessor", message)
         for handler in self.handlers.values():
             if not handler:
                 continue
-            
+
             handler.broadcast_message(message)
             break
 
     async def start(self):
         while True:
             self.process(await self.queue.get_async())
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/task_manager.py` & `jupyter_ai-0.9.0/jupyter_ai/task_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import asyncio
-import aiosqlite
 import os
-from typing import Optional, List
+from typing import List, Optional
 
+import aiosqlite
 from jupyter_core.paths import jupyter_data_dir
-from .models import ListTasksResponse, ListTasksEntry, DescribeTaskResponse, ListEnginesEntry
+
+from .models import (
+    DescribeTaskResponse,
+    ListEnginesEntry,
+    ListTasksEntry,
+    ListTasksResponse,
+)
+
 
 class TaskManager:
     db_path = os.path.join(jupyter_data_dir(), "ai_task_manager.db")
 
     def __init__(self, engines, default_tasks):
         self.engines = engines
         self.default_tasks = default_tasks
         self.db_initialized = asyncio.create_task(self.init_db())
- 
+
     async def init_db(self):
         async with aiosqlite.connect(self.db_path) as con:
             await con.execute(
                 "CREATE TABLE IF NOT EXISTS tasks ("
                 "id TEXT NOT NULL PRIMARY KEY, "
                 "name TEXT NOT NULL, "
                 "prompt_template TEXT NOT NULL, "
@@ -29,61 +36,63 @@
 
             # delete and recreate all default tasks. this ensures the default
             # tasks are all up-to-date.
             await con.execute("DELETE FROM tasks WHERE is_default = 1")
             for task in self.default_tasks:
                 await con.execute(
                     "INSERT INTO tasks (id, name, prompt_template, modality, insertion_mode, is_default) VALUES (?, ?, ?, ?, ?, ?)",
-                    (task["id"], task["name"], task["prompt_template"], task["modality"], task["insertion_mode"], 1)
+                    (
+                        task["id"],
+                        task["name"],
+                        task["prompt_template"],
+                        task["modality"],
+                        task["insertion_mode"],
+                        1,
+                    ),
                 )
-            
+
             await con.commit()
-    
+
     async def list_tasks(self) -> ListTasksResponse:
         await self.db_initialized
         async with aiosqlite.connect(self.db_path) as con:
-            cursor = await con.execute(
-                "SELECT id, name FROM tasks"
-            )
+            cursor = await con.execute("SELECT id, name FROM tasks")
             rows = await cursor.fetchall()
             tasks = []
 
             if not rows:
                 return tasks
-            
+
             for row in rows:
-                tasks.append(ListTasksEntry(
-                    id=row[0],
-                    name=row[1]
-                ))
-            
+                tasks.append(ListTasksEntry(id=row[0], name=row[1]))
+
             return ListTasksResponse(tasks=tasks)
-        
+
     async def describe_task(self, id: str) -> Optional[DescribeTaskResponse]:
         await self.db_initialized
         async with aiosqlite.connect(self.db_path) as con:
             cursor = await con.execute(
-                "SELECT name, prompt_template, modality, insertion_mode FROM tasks WHERE id = ?", (id,)
+                "SELECT name, prompt_template, modality, insertion_mode FROM tasks WHERE id = ?",
+                (id,),
             )
             row = await cursor.fetchone()
 
             if row is None:
                 return None
 
             # determine what engines are available for the task's modality
             engines: List[ListEnginesEntry] = []
             modality = row[2]
             for engine in self.engines.values():
                 if modality in engine.modalities:
                     engines.append(ListEnginesEntry(id=engine.id, name=engine.name))
-            
+
             # sort engines A-Z
             engines = sorted(engines, key=lambda engine: engine.name)
-            
+
             return DescribeTaskResponse(
                 name=row[0],
                 prompt_template=row[1],
                 modality=row[2],
                 insertion_mode=row[3],
-                engines=engines
+                engines=engines,
             )
-
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/tasks.py` & `jupyter_ai-0.9.0/jupyter_ai/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 from typing import List, TypedDict
 
+
 class DefaultTaskDefinition(TypedDict):
     id: str
     name: str
     prompt_template: str
     modality: str
     insertion_mode: str
 
+
 tasks: List[DefaultTaskDefinition] = [
     {
         "id": "explain-code",
         "name": "Explain code",
-        "prompt_template": "Explain the following Python 3 code. The first sentence must begin with the phrase \"The code below\".\n{body}",
+        "prompt_template": 'Explain the following Python 3 code. The first sentence must begin with the phrase "The code below".\n{body}',
         "modality": "txt2txt",
-        "insertion_mode": "above"
+        "insertion_mode": "above",
     },
     {
         "id": "generate-code",
         "name": "Generate code",
         "prompt_template": "Generate Python 3 code in Markdown according to the following definition.\n{body}",
         "modality": "txt2txt",
-        "insertion_mode": "below"
+        "insertion_mode": "below",
     },
     {
         "id": "explain-code-in-cells-above",
         "name": "Explain code in cells above",
-        "prompt_template": "Explain the following Python 3 code. The first sentence must begin with the phrase \"The code below\".\n{body}",
+        "prompt_template": 'Explain the following Python 3 code. The first sentence must begin with the phrase "The code below".\n{body}',
         "modality": "txt2txt",
-        "insertion_mode": "above-in-cells"
+        "insertion_mode": "above-in-cells",
     },
     {
         "id": "generate-code-in-cells-below",
         "name": "Generate code in cells below",
         "prompt_template": "Generate Python 3 code in Markdown according to the following definition.\n{body}",
         "modality": "txt2txt",
-        "insertion_mode": "below-in-cells"
+        "insertion_mode": "below-in-cells",
     },
     {
         "id": "freeform",
         "name": "Freeform prompt",
         "prompt_template": "{body}",
         "modality": "txt2txt",
-        "insertion_mode": "below"
-    }
+        "insertion_mode": "below",
+    },
 ]
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/ask.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/ask.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,79 @@
 import argparse
 from typing import Dict, List, Type
-from jupyter_ai_magics.providers import BaseProvider
 
 import ray
-from ray.util.queue import Queue
-
+from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor, Logger
+from jupyter_ai.models import HumanChatMessage
+from jupyter_ai_magics.providers import BaseProvider
 from langchain.chains import ConversationalRetrievalChain
 from langchain.schema import BaseRetriever, Document
-
-from jupyter_ai.models import HumanChatMessage
-from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor, Logger
+from ray.util.queue import Queue
 
 
 @ray.remote
 class AskActor(BaseActor):
     """Processes messages prefixed with /ask. This actor will
     send the message as input to a RetrieverQA chain, that
     follows the Retrieval and Generation (RAG) tehnique to
     query the documents from the index, and sends this context
     to the LLM to generate the final reply.
     """
 
     def __init__(self, reply_queue: Queue, log: Logger):
         super().__init__(reply_queue=reply_queue, log=log)
 
-        self.parser.prog = '/ask'
-        self.parser.add_argument('query', nargs=argparse.REMAINDER)
+        self.parser.prog = "/ask"
+        self.parser.add_argument("query", nargs=argparse.REMAINDER)
 
-    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+    def create_llm_chain(
+        self, provider: Type[BaseProvider], provider_params: Dict[str, str]
+    ):
         retriever = Retriever()
         self.llm = provider(**provider_params)
         self.chat_history = []
-        self.llm_chain = ConversationalRetrievalChain.from_llm(
-            self.llm,
-            retriever
-        )
+        self.llm_chain = ConversationalRetrievalChain.from_llm(self.llm, retriever)
 
     def _process_message(self, message: HumanChatMessage):
         args = self.parse_args(message)
         if args is None:
             return
-        query = ' '.join(args.query)
+        query = " ".join(args.query)
         if not query:
             self.reply(f"{self.parser.format_usage()}", message)
             return
-        
+
         self.get_llm_chain()
 
         try:
-            result = self.llm_chain({"question": query, "chat_history": self.chat_history})
-            response = result['answer']
+            # limit chat history to last 2 exchanges
+            self.chat_history = self.chat_history[-2:]
+            result = self.llm_chain(
+                {"question": query, "chat_history": self.chat_history}
+            )
+            response = result["answer"]
             self.chat_history.append((query, response))
             self.reply(response, message)
         except AssertionError as e:
             self.log.error(e)
-            response = """Sorry, an error occurred while reading the from the learned documents. 
-            If you have changed the embedding provider, try deleting the existing index by running 
+            response = """Sorry, an error occurred while reading the from the learned documents.
+            If you have changed the embedding provider, try deleting the existing index by running
             `/learn -d` command and then re-submitting the `learn <directory>` to learn the documents,
             and then asking the question again.
             """
             self.reply(response, message)
 
 
 class Retriever(BaseRetriever):
     """Wrapper retriever class to get relevant docs
     from the vector store, this is important because
     of inconsistent de-serialization of index when it's
     accessed directly from the ask actor.
     """
-    
+
     def get_relevant_documents(self, question: str):
         index_actor = ray.get_actor(ACTOR_TYPE.LEARN.value)
         docs = ray.get(index_actor.get_relevant_documents.remote(question))
         return docs
-    
+
     async def aget_relevant_documents(self, query: str) -> List[Document]:
-        return await super().aget_relevant_documents(query)
+        return await super().aget_relevant_documents(query)
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/base.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 import argparse
-from enum import Enum
-from uuid import uuid4
-import time
 import logging
-from typing import Dict, Optional, Type, Union
+import time
 import traceback
+from enum import Enum
+from typing import Dict, Optional, Type, Union
+from uuid import uuid4
 
-from jupyter_ai_magics.providers import BaseProvider
 import ray
-
+from jupyter_ai.models import AgentChatMessage, HumanChatMessage
+from jupyter_ai_magics.providers import BaseProvider
 from ray.util.queue import Queue
 
-from jupyter_ai.models import HumanChatMessage, AgentChatMessage
-
 Logger = Union[logging.Logger, logging.LoggerAdapter]
 
+
 class ACTOR_TYPE(str, Enum):
     # the top level actor that routes incoming messages to the appropriate actor
     ROUTER = "router"
 
     # the default actor that responds to messages using a language model
     DEFAULT = "default"
 
     ASK = "ask"
-    LEARN = 'learn'
-    MEMORY = 'memory'
-    GENERATE = 'generate'
-    PROVIDERS = 'providers'
-    CONFIG = 'config'
-    CHAT_PROVIDER = 'chat_provider'
-    EMBEDDINGS_PROVIDER = 'embeddings_provider'
+    LEARN = "learn"
+    MEMORY = "memory"
+    GENERATE = "generate"
+    PROVIDERS = "providers"
+    CONFIG = "config"
+    CHAT_PROVIDER = "chat_provider"
+    EMBEDDINGS_PROVIDER = "embeddings_provider"
+
 
 COMMANDS = {
-    '/ask': ACTOR_TYPE.ASK,
-    '/learn': ACTOR_TYPE.LEARN,
-    '/generate': ACTOR_TYPE.GENERATE
+    "/ask": ACTOR_TYPE.ASK,
+    "/learn": ACTOR_TYPE.LEARN,
+    "/generate": ACTOR_TYPE.GENERATE,
 }
 
-class BaseActor():
+
+class BaseActor:
     """Base actor implemented by actors that are called by the `Router`"""
 
-    def __init__(
-            self, 
-            log: Logger,
-            reply_queue: Queue
-        ):
+    def __init__(self, log: Logger, reply_queue: Queue):
         self.log = log
         self.reply_queue = reply_queue
         self.parser = argparse.ArgumentParser()
         self.llm = None
         self.llm_params = None
         self.llm_chain = None
         self.embeddings = None
@@ -59,63 +56,80 @@
         """Processes the message passed by the `Router`"""
         try:
             self._process_message(message)
         except Exception as e:
             formatted_e = traceback.format_exc()
             response = f"Sorry, something went wrong and I wasn't able to index that path.\n\n```\n{formatted_e}\n```"
             self.reply(response, message)
-    
+
     def _process_message(self, message: HumanChatMessage):
         """Processes the message passed by the `Router`"""
         raise NotImplementedError("Should be implemented by subclasses.")
-    
+
     def reply(self, response, message: Optional[HumanChatMessage] = None):
         m = AgentChatMessage(
             id=uuid4().hex,
             time=time.time(),
             body=response,
-            reply_to=message.id if message else ""
+            reply_to=message.id if message else "",
         )
         self.reply_queue.put(m)
 
     def get_llm_chain(self):
         actor = ray.get_actor(ACTOR_TYPE.CHAT_PROVIDER)
         lm_provider = ray.get(actor.get_provider.remote())
         lm_provider_params = ray.get(actor.get_provider_params.remote())
 
-        curr_lm_id = f'{self.llm.id}:{lm_provider_params["model_id"]}' if self.llm else None
-        next_lm_id = f'{lm_provider.id}:{lm_provider_params["model_id"]}' if lm_provider else None
+        curr_lm_id = (
+            f'{self.llm.id}:{lm_provider_params["model_id"]}' if self.llm else None
+        )
+        next_lm_id = (
+            f'{lm_provider.id}:{lm_provider_params["model_id"]}'
+            if lm_provider
+            else None
+        )
 
-        if not lm_provider:
+        if not lm_provider or not lm_provider_params:
             return None
-        
+
         if curr_lm_id != next_lm_id:
-            self.log.info(f"Switching chat language model from {curr_lm_id} to {next_lm_id}.")
+            self.log.info(
+                f"Switching chat language model from {curr_lm_id} to {next_lm_id}."
+            )
+            self.create_llm_chain(lm_provider, lm_provider_params)
+        elif self.llm_params != lm_provider_params:
+            self.log.info("Chat model params changed, updating the llm chain.")
             self.create_llm_chain(lm_provider, lm_provider_params)
+
         return self.llm_chain
-    
+
     def get_embeddings(self):
         actor = ray.get_actor(ACTOR_TYPE.EMBEDDINGS_PROVIDER)
         provider = ray.get(actor.get_provider.remote())
         embedding_params = ray.get(actor.get_provider_params.remote())
         embedding_model_id = ray.get(actor.get_model_id.remote())
-        
-        if not provider:
+
+        if not provider or not embedding_params:
             return None
-        
-        if embedding_model_id != self.embedding_model_id:
+
+        if (
+            embedding_model_id != self.embedding_model_id
+            or self.embeddings_params != embedding_params
+        ):
             self.embeddings = provider(**embedding_params)
 
         return self.embeddings
-    
-    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+
+    def create_llm_chain(
+        self, provider: Type[BaseProvider], provider_params: Dict[str, str]
+    ):
         raise NotImplementedError("Should be implemented by subclasses")
-    
+
     def parse_args(self, message):
-        args = message.body.split(' ')
+        args = message.body.split(" ")
         try:
             args = self.parser.parse_args(args[1:])
         except (argparse.ArgumentError, SystemExit) as e:
             response = f"{self.parser.format_usage()}"
             self.reply(response, message)
             return None
-        return args
+        return args
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/chat_provider.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/chat_provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from jupyter_ai.actors.base import Logger, ACTOR_TYPE
-from jupyter_ai.models import GlobalConfig
 import ray
+from jupyter_ai.actors.base import ACTOR_TYPE, Logger
+from jupyter_ai.models import GlobalConfig
 
-@ray.remote
-class ChatProviderActor():
 
+@ray.remote
+class ChatProviderActor:
     def __init__(self, log: Logger):
         self.log = log
         self.provider = None
         self.provider_params = None
 
     def update(self, config: GlobalConfig):
         model_id = config.model_provider_id
         actor = ray.get_actor(ACTOR_TYPE.PROVIDERS.value)
         local_model_id, provider = ray.get(
             actor.get_model_provider_data.remote(model_id)
         )
-        
+
         if not provider:
             raise ValueError(f"No provider and model found with '{model_id}'")
-        
+
         fields = config.fields.get(model_id, {})
-        provider_params = { "model_id": local_model_id, **fields }
-        
+        provider_params = {"model_id": local_model_id, **fields}
+
         auth_strategy = provider.auth_strategy
         if auth_strategy and auth_strategy.type == "env":
             api_keys = config.api_keys
             name = auth_strategy.name
             if name not in api_keys:
-                raise ValueError(f"Missing value for '{auth_strategy.name}' in the config.")
+                raise ValueError(
+                    f"Missing value for '{auth_strategy.name}' in the config."
+                )
             provider_params[name.lower()] = api_keys[name]
-            
+
         self.provider = provider
         self.provider_params = provider_params
 
     def get_provider(self):
         return self.provider
-    
+
     def get_provider_params(self):
-        return self.provider_params
+        return self.provider_params
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/config.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import json
 import os
+
+import ray
 from jupyter_ai.actors.base import ACTOR_TYPE, Logger
 from jupyter_ai.models import GlobalConfig
-import ray
 from jupyter_core.paths import jupyter_data_dir
 
 
 @ray.remote
-class ConfigActor():
-    """Provides model and embedding provider id along 
+class ConfigActor:
+    """Provides model and embedding provider id along
     with the credentials to authenticate providers.
     """
 
     def __init__(self, log: Logger):
         self.log = log
-        self.save_dir = os.path.join(jupyter_data_dir(), 'jupyter_ai')
-        self.save_path = os.path.join(self.save_dir, 'config.json')
+        self.save_dir = os.path.join(jupyter_data_dir(), "jupyter_ai")
+        self.save_path = os.path.join(self.save_dir, "config.json")
         self.config = None
         self._load()
 
     def update(self, config: GlobalConfig, save_to_disk: bool = True):
         self._update_chat_provider(config)
         self._update_embeddings_provider(config)
         if save_to_disk:
             self._save(config)
         self.config = config
-    
+
     def _update_chat_provider(self, config: GlobalConfig):
         if not config.model_provider_id:
             return
 
         actor = ray.get_actor(ACTOR_TYPE.CHAT_PROVIDER)
         ray.get(actor.update.remote(config))
 
@@ -39,23 +40,23 @@
 
         actor = ray.get_actor(ACTOR_TYPE.EMBEDDINGS_PROVIDER)
         ray.get(actor.update.remote(config))
 
     def _save(self, config: GlobalConfig):
         if not os.path.exists(self.save_dir):
             os.makedirs(self.save_dir)
-        
-        with open(self.save_path, 'w') as f:
+
+        with open(self.save_path, "w") as f:
             f.write(config.json())
 
     def _load(self):
         if os.path.exists(self.save_path):
-            with open(self.save_path, 'r', encoding='utf-8') as f:
+            with open(self.save_path, encoding="utf-8") as f:
                 config = GlobalConfig(**json.loads(f.read()))
                 self.update(config, False)
             return
-        
+
         # otherwise, create a new empty config file
         self.update(GlobalConfig(), True)
 
     def get_config(self):
-        return self.config
+        return self.config
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/default.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/default.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,72 @@
-from typing import Dict, Type, List
-import ray
+from typing import Dict, List, Type
 
+import ray
+from jupyter_ai.actors.base import ACTOR_TYPE, BaseActor
+from jupyter_ai.actors.memory import RemoteMemory
+from jupyter_ai.models import ChatMessage, ClearMessage, HumanChatMessage
+from jupyter_ai_magics.providers import BaseProvider
 from langchain import ConversationChain
 from langchain.prompts import (
-    ChatPromptTemplate, 
-    MessagesPlaceholder, 
+    ChatPromptTemplate,
     HumanMessagePromptTemplate,
-    SystemMessagePromptTemplate
-)
-from langchain.schema import (
-    AIMessage,
+    MessagesPlaceholder,
+    SystemMessagePromptTemplate,
 )
-
-from jupyter_ai.actors.base import BaseActor, ACTOR_TYPE
-from jupyter_ai.actors.memory import RemoteMemory
-from jupyter_ai.models import HumanChatMessage, ClearMessage, ChatMessage
-from jupyter_ai_magics.providers import BaseProvider
+from langchain.schema import AIMessage
 
 SYSTEM_PROMPT = """
 You are Jupyternaut, a conversational assistant living in JupyterLab to help users.
 You are not a language model, but rather an application built on a foundation model from {provider_name} called {local_model_id}.
 You are talkative and you provide lots of specific details from the foundation model's context.
 You may use Markdown to format your response.
 Code blocks must be formatted in Markdown.
 Math should be rendered with inline TeX markup, surrounded by $.
 If you do not know the answer to a question, answer truthfully by responding that you do not know.
 The following is a friendly conversation between you and a human.
 """.strip()
 
+
 @ray.remote
 class DefaultActor(BaseActor):
     def __init__(self, chat_history: List[ChatMessage], *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.memory = None
         self.chat_history = chat_history
 
-    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+    def create_llm_chain(
+        self, provider: Type[BaseProvider], provider_params: Dict[str, str]
+    ):
         llm = provider(**provider_params)
         self.memory = RemoteMemory(actor_name=ACTOR_TYPE.MEMORY)
-        prompt_template = ChatPromptTemplate.from_messages([
-            SystemMessagePromptTemplate.from_template(SYSTEM_PROMPT).format(provider_name=llm.name, local_model_id=llm.model_id),
-            MessagesPlaceholder(variable_name="history"),
-            HumanMessagePromptTemplate.from_template("{input}"),
-            AIMessage(content="")
-        ])
+        prompt_template = ChatPromptTemplate.from_messages(
+            [
+                SystemMessagePromptTemplate.from_template(SYSTEM_PROMPT).format(
+                    provider_name=llm.name, local_model_id=llm.model_id
+                ),
+                MessagesPlaceholder(variable_name="history"),
+                HumanMessagePromptTemplate.from_template("{input}"),
+                AIMessage(content=""),
+            ]
+        )
         self.llm = llm
         self.llm_chain = ConversationChain(
-            llm=llm,
-            prompt=prompt_template,
-            verbose=True,
-            memory=self.memory
+            llm=llm, prompt=prompt_template, verbose=True, memory=self.memory
         )
-    
+
     def clear_memory(self):
-        
         # clear chain memory
         if self.memory:
             self.memory.clear()
 
         # clear transcript for existing chat clients
         reply_message = ClearMessage()
         self.reply_queue.put(reply_message)
 
         # clear transcript for new chat clients
         if self.chat_history:
             self.chat_history.clear()
 
     def _process_message(self, message: HumanChatMessage):
         self.get_llm_chain()
-        response = self.llm_chain.predict(
-            input=message.body,
-            stop=["\nHuman:"]
-        )
+        response = self.llm_chain.predict(input=message.body, stop=["\nHuman:"])
         self.reply(response, message)
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/embeddings_provider.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/embeddings_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from jupyter_ai.actors.base import Logger, ACTOR_TYPE
-from jupyter_ai.models import GlobalConfig
 import ray
+from jupyter_ai.actors.base import ACTOR_TYPE, Logger
+from jupyter_ai.models import GlobalConfig
 
-@ray.remote
-class EmbeddingsProviderActor():
 
+@ray.remote
+class EmbeddingsProviderActor:
     def __init__(self, log: Logger):
         self.log = log
         self.provider = None
         self.provider_params = None
         self.model_id = None
 
     def update(self, config: GlobalConfig):
         model_id = config.embeddings_provider_id
         actor = ray.get_actor(ACTOR_TYPE.PROVIDERS.value)
         local_model_id, provider = ray.get(
             actor.get_embeddings_provider_data.remote(model_id)
         )
-        
+
         if not provider:
             raise ValueError(f"No provider and model found with '{model_id}'")
-        
+
         provider_params = {}
         provider_params[provider.model_id_key] = local_model_id
-        
+
         auth_strategy = provider.auth_strategy
         if auth_strategy and auth_strategy.type == "env":
             api_keys = config.api_keys
             name = auth_strategy.name
             if name not in api_keys:
-                raise ValueError(f"Missing value for '{auth_strategy.name}' in the config.")
+                raise ValueError(
+                    f"Missing value for '{auth_strategy.name}' in the config."
+                )
             provider_params[name.lower()] = api_keys[name]
-            
+
         self.provider = provider.provider_klass
         self.provider_params = provider_params
         previous_model_id = self.model_id
         self.model_id = model_id
-        
+
         if previous_model_id and previous_model_id != model_id:
             # delete the index
             actor = ray.get_actor(ACTOR_TYPE.LEARN)
             actor.delete_and_relearn.remote()
 
     def get_provider(self):
         return self.provider
-    
+
     def get_provider_params(self):
         return self.provider_params
-    
+
     def get_model_id(self):
-        return self.model_id
+        return self.model_id
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/generate.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/generate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import json
 import os
 from typing import Dict, Type
 
-import ray
-from ray.util.queue import Queue
-
-from langchain.llms import BaseLLM
-from langchain.prompts import PromptTemplate
-from langchain.llms import BaseLLM
-from langchain.chains import LLMChain
-
 import nbformat
-
-from jupyter_ai.models import HumanChatMessage
+import ray
 from jupyter_ai.actors.base import BaseActor, Logger
+from jupyter_ai.models import HumanChatMessage
 from jupyter_ai_magics.providers import BaseProvider, ChatOpenAINewProvider
+from langchain.chains import LLMChain
+from langchain.llms import BaseLLM
+from langchain.prompts import PromptTemplate
+from ray.util.queue import Queue
 
 schema = """{
   "$schema": "http://json-schema.org/draft-07/schema#",
   "type": "object",
   "properties": {
     "description": {
       "type": "string"
@@ -38,195 +34,202 @@
         "required": ["title", "content"]
       }
     }
   },
   "required": ["sections"]
 }"""
 
+
 class NotebookOutlineChain(LLMChain):
     """Chain to generate a notebook outline, with section titles and descriptions."""
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool=False) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "You are an AI that creates a detailed content outline for a Jupyter notebook on a given topic.\n"
             "Generate the outline as JSON data that will validate against this JSON schema:\n"
             "{schema}\n"
             "Here is a description of the notebook you will create an outline for: {description}\n"
             "Don't include an introduction or conclusion section in the outline, focus only on sections that will need code."
         )
         prompt = PromptTemplate(
             template=task_creation_template,
-            input_variables=[
-                "description",
-                "schema"
-            ],
+            input_variables=["description", "schema"],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
+
 def generate_outline(description, llm=None, verbose=False):
     """Generate an outline of sections given a description of a notebook."""
     chain = NotebookOutlineChain.from_llm(llm=llm, verbose=verbose)
     outline = chain.predict(description=description, schema=schema)
     return json.loads(outline)
 
+
 class CodeImproverChain(LLMChain):
     """Chain to improve source code."""
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool=False) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "Improve the following code and make sure it is valid. Make sure to return the improved code only - don't give an explanation of the improvements.\n"
             "{code}"
         )
         prompt = PromptTemplate(
             template=task_creation_template,
             input_variables=[
                 "code",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
+
 def improve_code(code, llm=None, verbose=False):
     """Improve source code using an LLM."""
     chain = CodeImproverChain.from_llm(llm=llm, verbose=verbose)
     improved_code = chain.predict(code=code)
-    improved_code = '\n'.join([line for line in improved_code.split('/n') if not line.startswith("```")])
+    improved_code = "\n".join(
+        [line for line in improved_code.split("/n") if not line.startswith("```")]
+    )
     return improved_code
 
+
 class NotebookSectionCodeChain(LLMChain):
     """Chain to generate source code for a notebook section."""
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool=False) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "You are an AI that writes code for a single section of a Jupyter notebook.\n"
             "Overall topic of the notebook: {description}\n"
             "Title of the notebook section: {title}\n"
             "Description of the notebok section: {content}\n"
             "Given this information, write all the code for this section and this section only."
             " Your output should be valid code with inline comments.\n"
             "Code in the notebook so far:\n"
             "{code_so_far}"
         )
         prompt = PromptTemplate(
             template=task_creation_template,
-            input_variables=[
-                "description",
-                "title",
-                "content",
-                "code_so_far"
-            ],
+            input_variables=["description", "title", "content", "code_so_far"],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
+
 def generate_code(outline, llm=None, verbose=False):
     """Generate source code for a section given a description of the notebook and section."""
     chain = NotebookSectionCodeChain.from_llm(llm=llm, verbose=verbose)
     code_so_far = []
-    for section in outline['sections']:
+    for section in outline["sections"]:
         code = chain.predict(
-            description=outline['description'],
-            title=section['title'],
-            content=section['content'],
-            code_so_far='\n'.join(code_so_far)
+            description=outline["description"],
+            title=section["title"],
+            content=section["content"],
+            code_so_far="\n".join(code_so_far),
         )
-        section['code'] = improve_code(code, llm=llm, verbose=verbose)
-        code_so_far.append(section['code'])
+        section["code"] = improve_code(code, llm=llm, verbose=verbose)
+        code_so_far.append(section["code"])
     return outline
 
+
 class NotebookSummaryChain(LLMChain):
     """Chain to generate a short summary of a notebook."""
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool=False) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "Create a markdown summary for a Jupyter notebook with the following content."
             " The summary should consist of a single paragraph.\n"
             "Content:\n{content}"
         )
         prompt = PromptTemplate(
             template=task_creation_template,
             input_variables=[
                 "content",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
+
 class NotebookTitleChain(LLMChain):
     """Chain to generate the title of a notebook."""
 
     @classmethod
-    def from_llm(cls, llm: BaseLLM, verbose: bool=False) -> LLMChain:
+    def from_llm(cls, llm: BaseLLM, verbose: bool = False) -> LLMChain:
         task_creation_template = (
             "Create a short, few word, descriptive title for a Jupyter notebook with the following content.\n"
             "Content:\n{content}"
         )
         prompt = PromptTemplate(
             template=task_creation_template,
             input_variables=[
                 "content",
             ],
         )
         return cls(prompt=prompt, llm=llm, verbose=verbose)
 
+
 def generate_title_and_summary(outline, llm=None, verbose=False):
     """Generate a title and summary of a notebook outline using an LLM."""
     summary_chain = NotebookSummaryChain.from_llm(llm=llm, verbose=verbose)
     title_chain = NotebookTitleChain.from_llm(llm=llm, verbose=verbose)
     summary = summary_chain.predict(content=outline)
     title = title_chain.predict(content=outline)
-    outline['summary'] = summary
-    outline['title'] = title.strip('"')
+    outline["summary"] = summary
+    outline["title"] = title.strip('"')
     return outline
 
+
 def create_notebook(outline):
     """Create an nbformat Notebook object for a notebook outline."""
     nbf = nbformat.v4
     nb = nbf.new_notebook()
-    nb['cells'].append(nbf.new_markdown_cell('# ' + outline['title']))
-    nb['cells'].append(nbf.new_markdown_cell('## Introduction'))
+    nb["cells"].append(nbf.new_markdown_cell("# " + outline["title"]))
+    nb["cells"].append(nbf.new_markdown_cell("## Introduction"))
     disclaimer = f"This notebook was created by [Jupyter AI](https://github.com/jupyterlab/jupyter-ai) with the following prompt:\n\n> {outline['prompt']}"
-    nb['cells'].append(nbf.new_markdown_cell(disclaimer))
-    nb['cells'].append(nbf.new_markdown_cell(outline['summary']))
+    nb["cells"].append(nbf.new_markdown_cell(disclaimer))
+    nb["cells"].append(nbf.new_markdown_cell(outline["summary"]))
 
-    for section in outline['sections'][1:]:
-        nb['cells'].append(nbf.new_markdown_cell('## ' + section['title']))
-        for code_block in section['code'].split('\n\n'):
-            nb['cells'].append(nbf.new_code_cell(code_block))
+    for section in outline["sections"][1:]:
+        nb["cells"].append(nbf.new_markdown_cell("## " + section["title"]))
+        for code_block in section["code"].split("\n\n"):
+            nb["cells"].append(nbf.new_code_cell(code_block))
     return nb
 
+
 @ray.remote
 class GenerateActor(BaseActor):
     """A Ray actor to generate a Jupyter notebook given a description."""
 
     def __init__(self, reply_queue: Queue, root_dir: str, log: Logger):
         super().__init__(log=log, reply_queue=reply_queue)
         self.root_dir = os.path.abspath(os.path.expanduser(root_dir))
         self.llm = None
 
-    def create_llm_chain(self, provider: Type[BaseProvider], provider_params: Dict[str, str]):
+    def create_llm_chain(
+        self, provider: Type[BaseProvider], provider_params: Dict[str, str]
+    ):
         llm = provider(**provider_params)
         self.llm = llm
         return llm
-  
+
     def _process_message(self, message: HumanChatMessage):
         self.get_llm_chain()
-        
+
         response = "👍 Great, I will get started on your notebook. It may take a few minutes, but I will reply here when the notebook is ready. In the meantime, you can continue to ask me other questions."
         self.reply(response, message)
 
         prompt = message.body
         outline = generate_outline(prompt, llm=self.llm, verbose=True)
         # Save the user input prompt, the description property is now LLM generated.
-        outline['prompt'] = prompt
+        outline["prompt"] = prompt
         outline = generate_code(outline, llm=self.llm, verbose=True)
         outline = generate_title_and_summary(outline, llm=self.llm)
         notebook = create_notebook(outline)
-        final_path = os.path.join(self.root_dir, outline['title'] + '.ipynb')
+        final_path = os.path.join(self.root_dir, outline["title"] + ".ipynb")
         nbformat.write(notebook, final_path)
         response = f"""🎉 I have created your notebook and saved it to the location {final_path}. I am still learning how to create notebooks, so please review all code before running it."""
         self.reply(response, message)
 
 
 # /generate notebook
 # Error handling
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/learn.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/learn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,73 @@
+import argparse
 import json
 import os
-import argparse
 import time
 from typing import List
 
 import ray
-from ray.util.queue import Queue
-
+from jupyter_ai.actors.base import BaseActor, Logger
+from jupyter_ai.document_loaders.directory import RayRecursiveDirectoryLoader
+from jupyter_ai.document_loaders.splitter import ExtensionSplitter, NotebookSplitter
+from jupyter_ai.models import HumanChatMessage, IndexedDir, IndexMetadata
 from jupyter_core.paths import jupyter_data_dir
-
 from langchain import FAISS
+from langchain.schema import Document
 from langchain.text_splitter import (
-    RecursiveCharacterTextSplitter, PythonCodeTextSplitter,
-    MarkdownTextSplitter, LatexTextSplitter
+    LatexTextSplitter,
+    MarkdownTextSplitter,
+    PythonCodeTextSplitter,
+    RecursiveCharacterTextSplitter,
 )
-from langchain.schema import Document
-
-from jupyter_ai.models import HumanChatMessage, IndexedDir, IndexMetadata
-from jupyter_ai.actors.base import BaseActor, Logger
-from jupyter_ai.document_loaders.directory import RayRecursiveDirectoryLoader
-from jupyter_ai.document_loaders.splitter import ExtensionSplitter, NotebookSplitter
+from ray.util.queue import Queue
 
+INDEX_SAVE_DIR = os.path.join(jupyter_data_dir(), "jupyter_ai", "indices")
+METADATA_SAVE_PATH = os.path.join(INDEX_SAVE_DIR, "metadata.json")
 
-INDEX_SAVE_DIR = os.path.join(jupyter_data_dir(), 'jupyter_ai', 'indices')
-METADATA_SAVE_PATH = os.path.join(INDEX_SAVE_DIR, 'metadata.json')
 
 @ray.remote
 class LearnActor(BaseActor):
-
     def __init__(self, reply_queue: Queue, log: Logger, root_dir: str):
         super().__init__(reply_queue=reply_queue, log=log)
         self.root_dir = root_dir
         self.chunk_size = 2000
         self.chunk_overlap = 100
-        self.parser.prog = '/learn'
-        self.parser.add_argument('-v', '--verbose', action='store_true')
-        self.parser.add_argument('-d', '--delete', action='store_true')
-        self.parser.add_argument('-l', '--list', action='store_true')
-        self.parser.add_argument('path', nargs=argparse.REMAINDER)
-        self.index_name = 'default'
+        self.parser.prog = "/learn"
+        self.parser.add_argument("-v", "--verbose", action="store_true")
+        self.parser.add_argument("-d", "--delete", action="store_true")
+        self.parser.add_argument("-l", "--list", action="store_true")
+        self.parser.add_argument("path", nargs=argparse.REMAINDER)
+        self.index_name = "default"
         self.index = None
         self.metadata = IndexMetadata(dirs=[])
-        
+
         if not os.path.exists(INDEX_SAVE_DIR):
             os.makedirs(INDEX_SAVE_DIR)
-        
-        self.load_or_create()    
-        
+
+        self.load_or_create()
+
     def _process_message(self, message: HumanChatMessage):
         if not self.index:
             self.load_or_create()
 
         # If index is not still there, embeddings are not present
         if not self.index:
-            self.reply("Sorry, please select an embedding provider before using the `/learn` command.")
+            self.reply(
+                "Sorry, please select an embedding provider before using the `/learn` command."
+            )
 
         args = self.parse_args(message)
         if args is None:
             return
 
         if args.delete:
             self.delete()
             self.reply(f"👍 I have deleted everything I previously learned.", message)
             return
-        
+
         if args.list:
             self.reply(self._build_list_response())
             return
 
         # Make sure the path exists.
         if not len(args.path) == 1:
             self.reply(f"{self.parser.format_usage()}", message)
@@ -77,128 +77,150 @@
         if not os.path.exists(load_path):
             response = f"Sorry, that path doesn't exist: {load_path}"
             self.reply(response, message)
             return
 
         if args.verbose:
             self.reply(f"Loading and splitting files for {load_path}", message)
-        
+
         self.learn_dir(load_path)
         self.save()
 
-        response = f"""🎉 I have learned documents at **{load_path}** and I am ready to answer questions about them. 
+        response = f"""🎉 I have learned documents at **{load_path}** and I am ready to answer questions about them.
         You can ask questions about these docs by prefixing your message with **/ask**."""
         self.reply(response, message)
 
     def _build_list_response(self):
         if not self.metadata.dirs:
             return "There are no docs that have been learned yet."
-        
+
         dirs = [dir.path for dir in self.metadata.dirs]
         dir_list = "\n- " + "\n- ".join(dirs) + "\n\n"
         message = f"""I can answer questions from docs in these directories:
         {dir_list}"""
         return message
 
     def learn_dir(self, path: str):
-        splitters={
-            '.py': PythonCodeTextSplitter(chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap),
-            '.md': MarkdownTextSplitter(chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap),
-            '.tex': LatexTextSplitter(chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap),
-            '.ipynb': NotebookSplitter(chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap)
+        splitters = {
+            ".py": PythonCodeTextSplitter(
+                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+            ),
+            ".md": MarkdownTextSplitter(
+                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+            ),
+            ".tex": LatexTextSplitter(
+                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+            ),
+            ".ipynb": NotebookSplitter(
+                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+            ),
         }
         splitter = ExtensionSplitter(
             splitters=splitters,
-            default_splitter=RecursiveCharacterTextSplitter(chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap)
+            default_splitter=RecursiveCharacterTextSplitter(
+                chunk_size=self.chunk_size, chunk_overlap=self.chunk_overlap
+            ),
         )
 
         loader = RayRecursiveDirectoryLoader(path)
         texts = loader.load_and_split(text_splitter=splitter)
         self.index.add_documents(texts)
         self._add_dir_to_metadata(path)
-    
+
     def _add_dir_to_metadata(self, path: str):
         dirs = self.metadata.dirs
         index = next((i for i, dir in enumerate(dirs) if dir.path == path), None)
         if not index:
             dirs.append(IndexedDir(path=path))
         self.metadata.dirs = dirs
 
     def delete_and_relearn(self):
         if not self.metadata.dirs:
             self.delete()
             return
         message = """🔔 Hi there, It seems like you have updated the embeddings model. For the **/ask**
-        command to work with the new model, I have to re-learn the documents you had previously 
+        command to work with the new model, I have to re-learn the documents you had previously
         submitted for learning. Please wait to use the **/ask** command until I am done with this task."""
         self.reply(message)
-        
+
         metadata = self.metadata
         self.delete()
         self.relearn(metadata)
 
     def delete(self):
         self.index = None
         self.metadata = IndexMetadata(dirs=[])
-        paths = [os.path.join(INDEX_SAVE_DIR, self.index_name+ext) for ext in ['.pkl', '.faiss']]
+        paths = [
+            os.path.join(INDEX_SAVE_DIR, self.index_name + ext)
+            for ext in [".pkl", ".faiss"]
+        ]
         for path in paths:
             if os.path.isfile(path):
                 os.remove(path)
         self.create()
 
     def relearn(self, metadata: IndexMetadata):
         # Index all dirs in the metadata
         if not metadata.dirs:
-            return    
-        
+            return
+
         for dir in metadata.dirs:
             self.learn_dir(dir.path)
-            
+
         self.save()
 
-        dir_list = "\n- " + "\n- ".join([dir.path for dir in self.metadata.dirs]) + "\n\n"
+        dir_list = (
+            "\n- " + "\n- ".join([dir.path for dir in self.metadata.dirs]) + "\n\n"
+        )
         message = f"""🎉 I am done learning docs in these directories:
-        {dir_list} I am ready to answer questions about them. 
+        {dir_list} I am ready to answer questions about them.
         You can ask questions about these docs by prefixing your message with **/ask**."""
         self.reply(message)
 
     def create(self):
         embeddings = self.get_embeddings()
         if not embeddings:
             return
-        self.index = FAISS.from_texts(["Jupyternaut knows about your filesystem, to ask questions first use the /learn command."], embeddings)
+        self.index = FAISS.from_texts(
+            [
+                "Jupyternaut knows about your filesystem, to ask questions first use the /learn command."
+            ],
+            embeddings,
+        )
         self.save()
 
     def save(self):
         if self.index is not None:
             self.index.save_local(INDEX_SAVE_DIR, index_name=self.index_name)
-        
+
         self.save_metadata()
 
     def save_metadata(self):
-        with open(METADATA_SAVE_PATH, 'w') as f:
+        with open(METADATA_SAVE_PATH, "w") as f:
             f.write(self.metadata.json())
 
     def load_or_create(self):
         embeddings = self.get_embeddings()
         if not embeddings:
             return
         if self.index is None:
             try:
-                self.index = FAISS.load_local(INDEX_SAVE_DIR, embeddings, index_name=self.index_name)
+                self.index = FAISS.load_local(
+                    INDEX_SAVE_DIR, embeddings, index_name=self.index_name
+                )
                 self.load_metadata()
             except Exception as e:
                 self.create()
 
     def load_metadata(self):
         if not os.path.exists(METADATA_SAVE_PATH):
-           return
-        
-        with open(METADATA_SAVE_PATH, 'r', encoding='utf-8') as f:
-            j = json.loads(f.read()) 
+            return
+
+        with open(METADATA_SAVE_PATH, encoding="utf-8") as f:
+            j = json.loads(f.read())
             self.metadata = IndexMetadata(**j)
 
     def get_relevant_documents(self, question: str) -> List[Document]:
         if self.index:
             docs = self.index.similarity_search(question)
             return docs
         return []
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/memory.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,89 @@
-from typing import Dict, Any, List
+from typing import Any, Dict, List
 
 import ray
+from jupyter_ai.actors.base import Logger
 from langchain.schema import BaseMemory
 from pydantic import PrivateAttr
 
-from jupyter_ai.actors.base import Logger
 
 @ray.remote
-class MemoryActor(object):
+class MemoryActor:
     """Turns any LangChain memory into a Ray actor.
-    
+
     The resulting actor can be used as LangChain memory in chains
     running in different actors by using RemoteMemory (below).
     """
-    
+
     def __init__(self, log: Logger, memory: BaseMemory):
         self.memory = memory
         self.log = log
-    
+
     def get_chat_memory(self):
         return self.memory.chat_memory
-    
+
     def get_output_key(self):
         return self.memory.output_key
-    
+
     def get_input_key(self):
         return self.memory.input_key
 
     def get_return_messages(self):
         return self.memory.return_messages
-    
+
     def get_memory_variables(self):
         return self.memory.memory_variables
 
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         return self.memory.save_context(inputs, outputs)
-    
+
     def clear(self):
         return self.memory.clear()
-    
+
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         return self.memory.load_memory_variables(inputs)
-    
 
-    
 
 class RemoteMemory(BaseMemory):
     """Wraps a MemoryActor into a LangChain memory class.
-    
+
     This enables you to use a single distributed memory across multiple
     Ray actors running different chains.
     """
-    
+
     actor_name: str
     _actor: Any = PrivateAttr()
 
     def __init__(self, **data):
         super().__init__(**data)
         self._actor = ray.get_actor(self.actor_name)
-        
+
     @property
     def memory_variables(self) -> List[str]:
         o = self._actor.get_memory_variables.remote()
         return ray.get(o)
-    
+
     @property
     def output_key(self):
         o = self._actor.get_output_key.remote()
         return ray.get(o)
-    
+
     @property
     def input_key(self):
         o = self._actor.get_input_key.remote()
         return ray.get(o)
-    
+
     @property
     def return_messages(self):
         o = self._actor.get_return_messages.remote()
         return ray.get(o)
-    
+
     def save_context(self, inputs: Dict[str, Any], outputs: Dict[str, str]) -> None:
         o = self._actor.save_context.remote(inputs, outputs)
         return ray.get(o)
-    
+
     def clear(self):
         self._actor.clear.remote()
-        
+
     def load_memory_variables(self, inputs: Dict[str, Any]) -> Dict[str, Any]:
         o = self._actor.load_memory_variables.remote(inputs)
-        return ray.get(o)
+        return ray.get(o)
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/providers.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 from typing import Optional, Tuple, Type
-from jupyter_ai_magics.embedding_providers import BaseEmbeddingsProvider
-from jupyter_ai_magics.providers import BaseProvider
-from jupyter_ai_magics.utils import decompose_model_id, load_embedding_providers, load_providers
+
 import ray
 from jupyter_ai.actors.base import BaseActor, Logger
+from jupyter_ai_magics.embedding_providers import BaseEmbeddingsProvider
+from jupyter_ai_magics.providers import BaseProvider
+from jupyter_ai_magics.utils import (
+    decompose_model_id,
+    load_embedding_providers,
+    load_providers,
+)
 from ray.util.queue import Queue
 
+
 @ray.remote
-class ProvidersActor():
+class ProvidersActor:
     """Actor that loads model and embedding providers from,
-    entry points. Also provides utility functions to get the 
+    entry points. Also provides utility functions to get the
     providers and provider class matching a provider id.
     """
-    
+
     def __init__(self, log: Logger):
         self.log = log
         self.model_providers = load_providers(log=log)
         self.embeddings_providers = load_embedding_providers(log=log)
 
     def get_model_providers(self):
         """Returns dictionary of registered LLM providers"""
         return self.model_providers
-    
+
     def get_model_provider_data(self, model_id: str) -> Tuple[str, Type[BaseProvider]]:
         """Returns the model provider class that matches the provider id"""
         provider_id, local_model_id = decompose_model_id(model_id, self.model_providers)
         provider = self.model_providers.get(provider_id, None)
         return local_model_id, provider
-    
+
     def get_embeddings_providers(self):
         """Returns dictionary of registered embedding providers"""
         return self.embeddings_providers
 
-    def get_embeddings_provider_data(self, model_id: str) -> Tuple[str, Type[BaseEmbeddingsProvider]]:
+    def get_embeddings_provider_data(
+        self, model_id: str
+    ) -> Tuple[str, Type[BaseEmbeddingsProvider]]:
         """Returns the embedding provider class that matches the provider id"""
-        provider_id, local_model_id = decompose_model_id(model_id, self.embeddings_providers)
+        provider_id, local_model_id = decompose_model_id(
+            model_id, self.embeddings_providers
+        )
         provider = self.embeddings_providers.get(provider_id, None)
         return local_model_id, provider
-    
-
-
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/actors/router.py` & `jupyter_ai-0.9.0/jupyter_ai/actors/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import ray
+from jupyter_ai.actors.base import ACTOR_TYPE, COMMANDS, BaseActor, Logger
 from ray.util.queue import Queue
 
-from jupyter_ai.actors.base import ACTOR_TYPE, COMMANDS, Logger, BaseActor
 
 @ray.remote
 class Router(BaseActor):
     def __init__(self, reply_queue: Queue, log: Logger):
         """Routes messages to the correct actor.
-        
-        To register new actors, add the actor type in the `ACTOR_TYPE` enum and 
+
+        To register new actors, add the actor type in the `ACTOR_TYPE` enum and
         add a corresponding command in the `COMMANDS` dictionary.
         """
         super().__init__(reply_queue=reply_queue, log=log)
 
     def _process_message(self, message):
-        
         # assign default actor
         default = ray.get_actor(ACTOR_TYPE.DEFAULT)
 
         if message.body.startswith("/"):
-            command = message.body.split(' ', 1)[0]
+            command = message.body.split(" ", 1)[0]
             if command in COMMANDS.keys():
                 actor = ray.get_actor(COMMANDS[command].value)
                 actor.process_message.remote(message)
-            if command == '/clear':
+            if command == "/clear":
                 actor = ray.get_actor(ACTOR_TYPE.DEFAULT)
                 actor.clear_memory.remote()
         else:
             default.process_message.remote(message)
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-0.9.0/jupyter_ai/document_loaders/splitter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,50 @@
+import copy
 from typing import List, Optional
 
 from langchain.schema import Document
-from langchain.text_splitter import TextSplitter, RecursiveCharacterTextSplitter, MarkdownTextSplitter
-import copy
+from langchain.text_splitter import (
+    MarkdownTextSplitter,
+    RecursiveCharacterTextSplitter,
+    TextSplitter,
+)
+
 
 class ExtensionSplitter(TextSplitter):
-    
     def __init__(self, splitters, default_splitter=None):
         self.splitters = splitters
         if default_splitter is None:
             self.default_splitter = RecursiveCharacterTextSplitter()
         else:
             self.default_splitter = default_splitter
-    
+
     def split_text(self, text: str, metadata=None):
-        splitter = self.splitters.get(metadata['extension'], self.default_splitter)
+        splitter = self.splitters.get(metadata["extension"], self.default_splitter)
         return splitter.split_text(text)
 
-    def create_documents(self, texts: List[str], metadatas: Optional[List[dict]] = None) -> List[Document]:
+    def create_documents(
+        self, texts: List[str], metadatas: Optional[List[dict]] = None
+    ) -> List[Document]:
         _metadatas = metadatas or [{}] * len(texts)
         documents = []
         for i, text in enumerate(texts):
             metadata = copy.deepcopy(_metadatas[i])
             for chunk in self.split_text(text, metadata):
-                new_doc = Document(
-                    page_content=chunk, metadata=metadata
-                )
+                new_doc = Document(page_content=chunk, metadata=metadata)
                 documents.append(new_doc)
         return documents
 
+
 import nbformat
 
+
 class NotebookSplitter(TextSplitter):
-    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.markdown_splitter = MarkdownTextSplitter(chunk_size=self._chunk_size, chunk_overlap=self._chunk_overlap)
-        
+        self.markdown_splitter = MarkdownTextSplitter(
+            chunk_size=self._chunk_size, chunk_overlap=self._chunk_overlap
+        )
+
     def split_text(self, text: str):
         nb = nbformat.reads(text, as_version=4)
-        md = '\n\n'.join([cell.source for cell in nb.cells])
+        md = "\n\n".join([cell.source for cell in nb.cells])
         return self.markdown_splitter.split_text(md)
-
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/package.json` & `jupyter_ai-0.9.0/jupyter_ai/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.974102564102564%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9095dd2e94ae47ffc04b.js'}}",*

 * * "'scripts'": '{\'dev-install\': \'pip install -e ".[dev,all]" && jupyter labextension develop . '*

 * *              "--overwrite && jupyter server extension enable jupyter_ai'}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -59,15 +59,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e77e7c805bbe3d26eec6.js",
+            "load": "static/remoteEntry.9095dd2e94ae47ffc04b.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -102,15 +102,15 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
+        "dev-install": "pip install -e \".[dev,all]\" && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
         "dev-uninstall": "pip uninstall jupyter_ai -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
@@ -126,9 +126,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745192307692306%*

 * *Differences: {"'scripts'": '{\'dev-install\': \'pip install -e ".[dev,all]" && jupyter labextension develop . '*

 * *              "--overwrite && jupyter server extension enable jupyter_ai'}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -97,15 +97,15 @@
         "build:lib": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
         "clean:labextension": "rimraf jupyter_ai/labextension",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
-        "dev-install": "pip install -e . && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
+        "dev-install": "pip install -e \".[dev,all]\" && jupyter labextension develop . --overwrite && jupyter server extension enable jupyter_ai",
         "dev-uninstall": "pip uninstall jupyter_ai -y",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
         "prettier": "jlpm prettier:base --write --list-different",
@@ -121,9 +121,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-0.9.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/00b26ac825e2095056396e0553b8ac26d3f8ad158c3826e28b4c45b385c4714a.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb54f1004170dd190a1f3db45d400fe68060df3e0897268.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/08ce98e51b04d58945a301e639e02b6998af29fdfd61a7b8afdd07bbfc479d4a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f9794560022dbb59654a7d86f187aa0c81495ad42d3a7308.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f1a58c4a112fdca8aae769b6ba11429af1d98b1b6cb3a.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8ce073092411baf9438f6739465693ff18b0f9d20b021.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee561d53d10fde8f7489e798257ff449c5d37c197435605.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c5f52371fa5c63d8324f4a38d22cd573e6ea3a3fd0cf8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf099c088b1cf64bd27516a6e07f4684344873564bb66a67.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8f60a597c436e075c114385652b7cbeb0dec0421291b3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc7f6b435a74e1379b0d46104a8530286b60ff49369ea0.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/253.0b5d158f3577d0bfbee5.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/253.4cb04dcfead6f07b8e7c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [253], {
         30253: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => me
             });
-            var r = n(96175),
-                o = n(75884),
+            var r = n(97638),
+                o = n(64270),
                 l = n(56271),
                 i = n.n(l),
-                a = n(49764),
+                a = n(56303),
                 s = n(53959),
                 c = n(35048),
                 d = n(13264),
                 u = n(28504),
                 m = n(28066),
                 h = n(53626);
 
@@ -160,24 +160,24 @@
                 v = n.n(f),
                 y = n(96707),
                 E = n.n(y),
                 _ = n(40532),
                 b = n.n(_),
                 C = (n(38662), n(55351)),
                 x = n(7464),
-                S = n(6277);
-            const w = "jp-ai-code";
+                w = n(6277);
+            const S = "jp-ai-code";
 
             function k({
                 className: e,
                 children: t,
                 ...n
             }) {
                 return i().createElement("code", Object.assign({}, n, {
-                    className: (0, S.Z)(w, e)
+                    className: (0, w.Z)(S, e)
                 }), t)
             }
             var j;
             ! function(e) {
                 e[e.None = 0] = "None", e[e.Copying = 1] = "Copying", e[e.Copied = 2] = "Copied"
             }(j || (j = {}));
             const I = {
@@ -195,15 +195,15 @@
                     [o, a] = (0, l.useState)(j.None);
                 return i().createElement(c.Box, {
                     sx: {
                         display: "flex",
                         flexDirection: "column"
                     }
                 }, i().createElement(C.Prism, Object.assign({}, n, {
-                    className: (0, S.Z)(n.className, w),
+                    className: (0, w.Z)(n.className, S),
                     children: r,
                     style: x.Z,
                     language: e,
                     PreTag: "div"
                 })), i().createElement(c.Button, {
                     onClick: async () => {
                         a(j.Copying);
@@ -250,22 +250,22 @@
                     return null == e || e.on("change", t), () => {
                         null == e || e.off("change", t)
                     }
                 }), [e]), e ? i().createElement(M.Provider, {
                     value: n
                 }, t) : t
             }
-            var A = n(78667);
+            var A = n(61745);
             const N = new A.LabIcon({
                     name: "jupyter-ai::chat",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
                 }),
                 T = new A.LabIcon({
                     name: "jupyter-ai::jupyternaut",
-                    svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>'
+                    svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>\n'
                 }).react;
 
             function R(e) {
                 var t;
                 const n = (0, l.useContext)(M),
                     r = {
                         height: "24px",
@@ -439,16 +439,16 @@
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }), e.children))
             }
-            var O, Z, D = n(83058),
-                J = n(11872);
+            var O, Z, D = n(344),
+                J = n(15139);
             async function V(e = "", t = {}) {
                 const n = J.ServerConnection.makeSettings(),
                     r = D.URLExt.join(n.baseUrl, "api/ai", e);
                 let o;
                 try {
                     o = await J.ServerConnection.makeRequest(r, t, n)
                 } catch (e) {
@@ -515,28 +515,28 @@
                 var e;
                 const [t, n] = (0, l.useState)(Z.Loading), [r, o] = (0, l.useState)(), [a, d] = (0, l.useState)(), [u, m] = (0, l.useState)(), [h, p] = (0, l.useState)(), [g, f] = (0, l.useState)({
                     model_provider_id: null,
                     embeddings_provider_id: null,
                     api_keys: {},
                     send_with_shift_enter: null,
                     fields: {}
-                }), [v, y] = (0, l.useState)(!1), [E, _] = (0, l.useState)(), [b, C] = (0, l.useState)(!1), [x, S] = (0, l.useState)("*"), w = (0, l.useMemo)((() => {
+                }), [v, y] = (0, l.useState)(!1), [E, _] = (0, l.useState)(), [b, C] = (0, l.useState)(!1), [x, w] = (0, l.useState)("*"), S = (0, l.useMemo)((() => {
                     if (g.model_provider_id && u) return K(g.model_provider_id, u)
-                }), [g.model_provider_id, u]), k = (0, l.useMemo)((() => g.model_provider_id && w ? (null == w ? void 0 : w.registry) ? `${w.id}:${x}` : g.model_provider_id : null), [g.model_provider_id, w, u, x]);
+                }), [g.model_provider_id, u]), k = (0, l.useMemo)((() => g.model_provider_id && S ? (null == S ? void 0 : S.registry) ? `${S.id}:${x}` : g.model_provider_id : null), [g.model_provider_id, S, u, x]);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         try {
                             const [e, t, r] = await Promise.all([O.getConfig(), O.listLmProviders(), O.listEmProviders()]);
                             if (d(e), m(t), p(r), function(e, t) {
                                     var n, r;
                                     return null !== (r = null === (n = K(e, t)) || void 0 === n ? void 0 : n.registry) && void 0 !== r && r
                                 }(e.model_provider_id, t)) {
                                 C(!0);
                                 const t = U(e.model_provider_id);
-                                S(function(e) {
+                                w(function(e) {
                                     if (!e) return null;
                                     const t = e.split(":");
                                     return t[t.length - 1]
                                 }(e.model_provider_id)), f({
                                     ...e,
                                     model_provider_id: `${t}:*`
                                 })
@@ -570,15 +570,16 @@
                     }
                 }, i().createElement(c.CircularProgress, null)) : t !== Z.FetchError && u && h && a ? i().createElement(s.Z, {
                     sx: {
                         padding: 4,
                         boxSizing: "border-box",
                         "& > .MuiAlert-root": {
                             marginBottom: 2
-                        }
+                        },
+                        overflowY: "auto"
                     }
                 }, t === Z.SubmitError && i().createElement(c.Alert, {
                     severity: "error"
                 }, E ? `An error occurred. Error details:\n\n${E}` : "An unknown error occurred. Check the console for more details."), t === Z.Success && i().createElement(c.Alert, {
                     severity: "success"
                 }, "Settings saved successfully."), i().createElement("h2", {
                     className: "jp-ai-ChatSettings-header"
@@ -587,36 +588,36 @@
                     label: "Language model",
                     onChange: e => {
                         f((t => ({
                             ...t,
                             model_provider_id: e.target.value
                         })));
                         const t = K(e.target.value, u);
-                        (null == t ? void 0 : t.registry) ? (C(!0), S("*")) : C(!1)
+                        (null == t ? void 0 : t.registry) ? (C(!0), w("*")) : C(!1)
                     },
                     MenuProps: {
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }, i().createElement(c.MenuItem, {
                     value: "null"
                 }, "None"), u.providers.map((e => e.models.map((t => i().createElement(c.MenuItem, {
                     value: `${e.id}:${t}`
                 }, e.name, " :: ", t)))))), b && i().createElement(c.TextField, {
                     label: "Local model ID",
                     value: x,
-                    onChange: e => S(e.target.value),
+                    onChange: e => w(e.target.value),
                     fullWidth: !0
                 }), k && i().createElement(G, {
                     gmid: k,
                     config: g,
                     setConfig: f,
-                    fields: null == w ? void 0 : w.fields
+                    fields: null == S ? void 0 : S.fields
                 }), i().createElement("h2", {
                     className: "jp-ai-ChatSettings-header"
                 }, "Embedding model"), i().createElement(H, {
                     value: g.embeddings_provider_id,
                     label: "Embedding model",
                     onChange: e => f((t => ({
                         ...t,
@@ -743,30 +744,30 @@
                         body: JSON.stringify(e)
                     })
                 }
             }(O || (O = {})),
             function(e) {
                 e[e.Loading = 0] = "Loading", e[e.Ready = 1] = "Ready", e[e.FetchError = 2] = "FetchError", e[e.SubmitError = 3] = "SubmitError", e[e.Success = 4] = "Success"
             }(Z || (Z = {}));
-            const q = i().createContext([null, () => {}]);
+            const Y = i().createContext([null, () => {}]);
 
-            function Y({
+            function q({
                 selectionWatcher: e,
                 children: t
             }) {
                 const [n, r] = (0, l.useState)(null);
                 (0, l.useEffect)((() => {
                     e.selectionChanged.connect(((e, t) => {
                         r(t)
                     }))
                 }), []);
                 const o = (0, l.useCallback)((t => {
                     e.replaceSelection(t)
                 }), [e]);
-                return i().createElement(q.Provider, {
+                return i().createElement(Y.Provider, {
                     value: [n, o]
                 }, t)
             }
 
             function X(e) {
                 const t = (0, l.useMemo)((() => "jupyter-ai-scroll-container-" + Date.now().toString()), []);
                 return (0, l.useEffect)((() => {
@@ -803,15 +804,15 @@
                 }))
             }
 
             function ee({
                 chatHandler: e,
                 setChatView: t
             }) {
-                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(q), [E, _] = (0, l.useState)(!0);
+                const [n, r] = (0, l.useState)([]), [o, a] = (0, l.useState)(!1), [u, m] = (0, l.useState)(!0), [h, p] = (0, l.useState)(!1), [g, f] = (0, l.useState)(""), [v, y] = (0, l.useContext)(Y), [E, _] = (0, l.useState)(!0);
                 return (0, l.useEffect)((() => {
                     !async function() {
                         var t;
                         try {
                             const [n, o] = await Promise.all([e.getHistory(), O.getConfig()]);
                             _(null !== (t = o.send_with_shift_enter) && void 0 !== t && t), r(n.messages), o.model_provider_id || a(!0)
                         } catch (e) {
@@ -886,15 +887,15 @@
                     sendWithShiftEnter: E
                 }))
             }
             var te;
 
             function ne(e) {
                 const [t, n] = (0, l.useState)(e.chatView || te.Chat);
-                return i().createElement(g, null, i().createElement(Y, {
+                return i().createElement(g, null, i().createElement(q, {
                     selectionWatcher: e.selectionWatcher
                 }, i().createElement(F, {
                     globalAwareness: e.globalAwareness
                 }, i().createElement(s.Z, {
                     sx: {
                         width: "100%",
                         height: "100%",
@@ -915,18 +916,18 @@
                 }, i().createElement(d.Z, null)) : i().createElement(s.Z, null)), t === te.Chat && i().createElement(ee, {
                     chatHandler: e.chatHandler,
                     setChatView: n
                 }), t === te.Settings && i().createElement(Q, null)))))
             }! function(e) {
                 e[e.Chat = 0] = "Chat", e[e.Settings = 1] = "Settings"
             }(te || (te = {}));
-            var re = n(26676),
-                oe = n(36705),
-                le = n(82883),
-                ie = n(76779),
+            var re = n(68020),
+                oe = n(59235),
+                le = n(40763),
+                ie = n(80127),
                 ae = n(78918),
                 se = n(71840);
 
             function ce(e) {
                 var t;
                 if (!(e instanceof re.DocumentWidget)) return null;
                 let n;
@@ -968,32 +969,32 @@
                     const e = this._selection,
                         t = function(e) {
                             var t;
                             const n = ce(e);
                             if (!(n && e instanceof re.DocumentWidget)) return null;
                             let r;
                             e.content instanceof ie.Notebook && (r = null === (t = e.content.activeCell) || void 0 === t ? void 0 : t.model.id);
+                            const o = n.getSelection();
                             let {
-                                start: o,
-                                end: l,
-                                ...i
-                            } = n.getSelection();
-                            const a = n.getOffsetAt(o),
-                                s = n.getOffsetAt(l),
+                                start: l,
+                                end: i
+                            } = o;
+                            const a = n.getOffsetAt(l),
+                                s = n.getOffsetAt(i),
                                 c = n.model.sharedModel.getSource().substring(a, s);
-                            return a > s && ([o, l] = [l, o]), {
-                                ...i,
-                                start: o,
-                                end: l,
+                            return c ? (a > s && ([l, i] = [i, l]), {
+                                ...o,
+                                start: l,
+                                end: i,
                                 text: c,
                                 widgetId: e.id,
                                 ...r && {
                                     cellId: r
                                 }
-                            }
+                            }) : null
                         }(this._mainAreaWidget);
                     (null == e ? void 0 : e.text) !== (null == t ? void 0 : t.text) && (this._selection = t, this._selectionChanged.emit(t))
                 }
             }
             class ue {
                 constructor(e = {}) {
                     var t;
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/30da91e84c893f875e252689faebdc590b2871145e8adc7f9a9d4dbd8ce0b251.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/341.f8070bd4be2814acfc0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/342.d3a98882c7231544e992.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/365.d20799d043a171f06d37.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/380.367f93b5ced659dcbadd.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/3931dd81faed86ba021bb2bbdc36f5bed9a38d6b4f4077aca59b265aa1b02083.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/51814d270d06ff0255dba0799994fa4d8c84d11f09951d47595f4abb1f3602dc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/527.96409770f04a31a6ae7e.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/598.168be006d4b42d34521a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/5e28753be717dac97f559f49bc10be9cf3c124ddcabda6659d11cb68febc6463.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/643.ca949b2ea9d252cbcc23.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/643.23e0a9c561346f879c77.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -9,26 +9,26 @@
                 i = t.n(r),
                 o = t(83055),
                 a = t(98814),
                 s = t(22299),
                 c = i()((function(e) {
                     return e[1]
                 }));
-            c.i(o.Z), c.i(a.Z), c.i(s.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/", ""]);
+            c.i(o.Z), c.i(a.Z), c.i(s.Z), c.push([e.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n", ""]);
             const l = c
         },
         22299: (e, n, t) => {
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
                 i = t.n(r)()((function(e) {
                     return e[1]
                 }));
-            i.push([e.id, ".jp-ai-ChatSettings-header {\n    font-size: var(--jp-ui-font-size3);\n    font-weight: 400;\n    color: var(--jp-ui-font-color1);\n}", ""]);
+            i.push([e.id, ".jp-ai-ChatSettings-header {\n  font-size: var(--jp-ui-font-size3);\n  font-weight: 400;\n  color: var(--jp-ui-font-color1);\n}\n", ""]);
             const o = i
         },
         83055: (e, n, t) => {
             t.d(n, {
                 Z: () => o
             });
             var r = t(82609),
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/675.e2778aeb06575c94bca0.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f0e8deb48684dd01e7f04ea2813267577afb906de1d13.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec58bf0fba302cce448938e7fc020a5e31f8a952eee1342.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/693.970d9a45469683adfff5.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/703.3d0d8b7012529f0dd511.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/70ee1f64a20f2048c21940ef46d0144fd215baa953ca69afd1e31e98544f708f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/71d517d67827787cfabdf186914cc3358eda539e37931941f2b2fd4a21f68c0b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/74444efd593c005e3f4573b44524704c0af0a937fe911cca9e94068d0d140d3f.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde9027c6d7814decce4d3b822a11192a42a20e2e973264.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/819.5279f5daf1d1f505f15f.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/850c0af5c2238497febaf5e461d880bf458c341f42f4f330f1b1ab5698b1998e.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/860.03421bb262ea8bfa0af1.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/861.c7c12ea31e8b5552473d.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/8a8d244581371912b8f3f5a23e2437cb2a59cd9bcaebb0346e722c05737a2571.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/900.899d3fbf00938382f665.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/9163df9c7122432e6495b4229fa9071cf9ae86a758ae5efc4924ec2e1a6dbce1.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ace3ac5c61ff1692102f0f31d02b69347fba35dcb75bf2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8c63e1d1c99b10427d0a4df4201cb44513b226951a22b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/97479ca6cce906abc961ecac96faa5f9ca2e61b8e7670d475826bcdee9a7c267.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f44984a807cf7aa16e13545fd0875fc07c6c65f99e715b.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124082246fbfcca4091e36385d4ec6ed1df67375dad50fb.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0db3a08842ebf1d732c6eb4e4bf44913613bed4fc4e39b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975adb8959c37ed49b94acbc4ae436db9ce9e20287e4a64c.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9321dc17213fc40d4d04c79688c1d43f2cf316abd7866.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337623d83d8dc4b868f242a9ad476237d6f8d1e0f168cdc.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c647367d1dd4e162468717d020e1fc0f1dc5c26ebfdffbe55261713bf88c5877.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1639c7da4334f0e7dec81b42b11213b5e25ef671bb822.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/d0332f52868370fd83ae7fa46470f90c8f2eab2fcf12bc4f88080b340c95a830.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd5f74a4c467f123a8a73931cd435889f08ffaf9bf947a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8460d561f4df5f501b90c804ad3c6cec65fe322351ab1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5afd5844b5d0321b22351febc720e0de8b8723527609f7.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc1bfe5add36262c6866b0faab24fa75740e1b98577a62.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/ece03cfd83e22c212cdef66feb8442d25a083beb988db3f1883f3f9738d750ba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c0666b2e210da37b7e49fa7fbbf3eeb11db5f693dacfbb7.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c081ceb577abd864eb00a612f7ac1620dd6915fad2ef5aa.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5185199bd2443ecb2b0dead96d88674b5a2c12be24bdf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d1e900e4e3710e438deb05a842486045ba0a3e616a4ad.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/f9377ab0271cda59af24bcffbd46a4d0c8a3572ffafdbb38de2ad5ea7b0d5ee5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/remoteEntry.e77e7c805bbe3d26eec6.js` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/remoteEntry.9095dd2e94ae47ffc04b.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, f, d, u, c, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
+    var e, r, t, a, o, n, i, l, f, u, c, d, s, p, h, b, m, v, y, g, j, P, w, k, _, O, S = {
             22399: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
                         "./extension": () => Promise.all([t.e(341), t.e(380), t.e(271), t.e(963), t.e(253)]).then((() => () => t(30253))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -56,49 +56,49 @@
         return n.default = () => t, x.d(o, n), o
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
-        253: "0b5d158f3577d0bfbee5",
+        253: "4cb04dcfead6f07b8e7c",
         271: "69215afaecf754ef22b8",
         296: "c1fab29ee6698d164796",
         341: "f8070bd4be2814acfc0d",
         342: "d3a98882c7231544e992",
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        643: "ca949b2ea9d252cbcc23",
+        643: "23e0a9c561346f879c77",
         675: "e2778aeb06575c94bca0",
         693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "c7c12ea31e8b5552473d",
         900: "899d3fbf00938382f665",
         963: "59c8f2feb6aaf0b34378"
     } [e] + ".js?v=" + {
-        253: "0b5d158f3577d0bfbee5",
+        253: "4cb04dcfead6f07b8e7c",
         271: "69215afaecf754ef22b8",
         296: "c1fab29ee6698d164796",
         341: "f8070bd4be2814acfc0d",
         342: "d3a98882c7231544e992",
         365: "d20799d043a171f06d37",
         380: "367f93b5ced659dcbadd",
         407: "6b1f897f3ceb4355d6ac",
         456: "3766abc0ca49db318bcd",
         527: "96409770f04a31a6ae7e",
         564: "43eaeac5fe02580e918d",
         598: "168be006d4b42d34521a",
-        643: "ca949b2ea9d252cbcc23",
+        643: "23e0a9c561346f879c77",
         675: "e2778aeb06575c94bca0",
         693: "970d9a45469683adfff5",
         703: "3d0d8b7012529f0dd511",
         819: "5279f5daf1d1f505f15f",
         860: "03421bb262ea8bfa0af1",
         861: "c7c12ea31e8b5552473d",
         900: "899d3fbf00938382f665",
@@ -111,32 +111,32 @@
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", x.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), d = 0; d < f.length; d++) {
-                    var u = f[d];
-                    if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == a + o) {
-                        i = u;
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var c = f[u];
+                    if (c.getAttribute("src") == e || c.getAttribute("data-webpack") == a + o) {
+                        i = c;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
-            var c = (r, a) => {
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(c.bind(null, void 0, {
+                s = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -158,15 +158,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     f = [];
-                return "default" === t && (l("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "0.8.0", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(253)]).then((() => () => x(30253))))), l("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@emotion/react", "11.11.0", (() => Promise.all([x.e(296), x.e(527), x.e(271), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(271), x.e(564), x.e(407)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "0.9.0", (() => Promise.all([x.e(341), x.e(380), x.e(271), x.e(963), x.e(253)]).then((() => () => x(30253))))), l("@mui/material", "5.13.1", (() => Promise.all([x.e(296), x.e(860), x.e(341), x.e(271), x.e(564), x.e(963), x.e(456)]).then((() => () => x(30860))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(271)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(271)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -216,97 +216,97 @@
     }, l = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
             for (var n = 0, i = 1, f = !0;; i++, n++) {
-                var d, u, c = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (u = (typeof(d = r[n]))[0])) return !f || ("u" == c ? i > t && !a : "" == c != a);
-                if ("u" == u) {
-                    if (!f || "u" != c) return !1
+                var u, c, d = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= r.length || "o" == (c = (typeof(u = r[n]))[0])) return !f || ("u" == d ? i > t && !a : "" == d != a);
+                if ("u" == c) {
+                    if (!f || "u" != d) return !1
                 } else if (f)
-                    if (c == u)
+                    if (d == c)
                         if (i <= t) {
-                            if (d != e[i]) return !1
+                            if (u != e[i]) return !1
                         } else {
-                            if (a ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (f = !1)
+                            if (a ? u > e[i] : u < e[i]) return !1;
+                            u != e[i] && (f = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != d && "n" != d) {
                     if (a || i <= t) return !1;
                     f = !1, i--
                 } else {
-                    if (i <= t || u < c != a) return !1;
+                    if (i <= t || c < d != a) return !1;
                     f = !1
-                } else "s" != c && "n" != c && (f = !1, i--)
+                } else "s" != d && "n" != d && (f = !1, i--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
             var h = e[n];
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
         return !!p()
     }, f = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, u = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
-    }, u = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
-        var o = u(e, t);
-        return l(a, o) || b(c(e, t, o, a)), v(e[t][o])
+    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
+        var o = c(e, t);
+        return l(a, o) || b(d(e, t, o, a)), v(e[t][o])
     }, p = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !l(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, h = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + i(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, b = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         b(h(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), g = (y = e => function(r, t, a, o) {
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
-    })(((e, r, t, a) => r && x.o(r, t) ? v(d(r, t)) : a())), j = y(((e, r, t, a) => (f(e, t), v(p(r, t, a) || m(r, e, t, a) || d(r, t))))), P = y(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && x.o(r, t) ? v(u(r, t)) : a())), j = y(((e, r, t, a) => (f(e, t), v(p(r, t, a) || m(r, e, t, a) || u(r, t))))), P = y(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && p(r, t, a);
         return n ? v(n) : o()
     })), k = {}, _ = {
         56271: () => P("default", "react", [1, 17, 0, 1]),
         79510: () => w("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([x.e(296), x.e(527), x.e(365)]).then((() => () => x(26527))))),
         92764: () => w("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([x.e(675), x.e(564), x.e(407)]).then((() => () => x(52675))))),
-        11872: () => P("default", "@jupyterlab/services", [1, 6, 6, 4]),
-        26676: () => j("default", "@jupyterlab/docregistry", [1, 3, 6, 4]),
+        344: () => P("default", "@jupyterlab/coreutils", [1, 5, 6, 5]),
+        15139: () => P("default", "@jupyterlab/services", [1, 6, 6, 5]),
         30535: () => w("default", "react-markdown", [1, 8, 0, 6], (() => Promise.all([x.e(693), x.e(861)]).then((() => () => x(81861))))),
         35048: () => w("default", "@mui/material", [1, 5, 11, 0], (() => Promise.all([x.e(296), x.e(860), x.e(564), x.e(456)]).then((() => () => x(30860))))),
-        36705: () => P("default", "@jupyterlab/codemirror", [1, 3, 6, 4]),
         40532: () => w("default", "rehype-katex", [1, 6, 0, 2], (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))),
-        49764: () => P("default", "@jupyterlab/apputils", [1, 3, 6, 4]),
+        40763: () => P("default", "@jupyterlab/fileeditor", [1, 3, 6, 5]),
         55351: () => w("default", "react-syntax-highlighter", [1, 15, 5, 0], (() => x.e(598).then((() => () => x(95598))))),
+        56303: () => P("default", "@jupyterlab/apputils", [1, 3, 6, 5]),
+        59235: () => P("default", "@jupyterlab/codemirror", [1, 3, 6, 5]),
+        61745: () => P("default", "@jupyterlab/ui-components", [1, 3, 6, 5]),
+        64270: () => P("default", "@jupyterlab/collaboration", [1, 3, 6, 5]),
+        68020: () => j("default", "@jupyterlab/docregistry", [1, 3, 6, 5]),
         71840: () => P("default", "@lumino/signaling", [1, 1, 10, 0]),
-        75884: () => P("default", "@jupyterlab/collaboration", [1, 3, 6, 4]),
-        76779: () => P("default", "@jupyterlab/notebook", [1, 3, 6, 4]),
-        78667: () => P("default", "@jupyterlab/ui-components", [1, 3, 6, 4]),
         78918: () => P("default", "@lumino/algorithm", [1, 1, 9, 0]),
-        82883: () => P("default", "@jupyterlab/fileeditor", [1, 3, 6, 4]),
-        83058: () => P("default", "@jupyterlab/coreutils", [1, 5, 6, 4]),
-        96175: () => P("default", "@jupyterlab/application", [1, 3, 6, 4]),
+        80127: () => P("default", "@jupyterlab/notebook", [1, 3, 6, 5]),
         96707: () => w("default", "remark-math", [1, 5, 1, 1], (() => x.e(703).then((() => () => x(7703))))),
+        97638: () => P("default", "@jupyterlab/application", [1, 3, 6, 5]),
         17564: () => g("default", "@emotion/react", (() => Promise.all([x.e(296), x.e(527), x.e(819)]).then((() => () => x(26527))))),
         24407: () => w("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([x.e(296), x.e(527)]).then((() => () => x(26527))))),
         14456: () => P("default", "react-dom", [1, 17, 0, 1])
     }, O = {
-        253: [11872, 26676, 30535, 35048, 36705, 40532, 49764, 55351, 71840, 75884, 76779, 78667, 78918, 82883, 83058, 96175, 96707],
+        253: [344, 15139, 30535, 35048, 40532, 40763, 55351, 56303, 59235, 61745, 64270, 68020, 71840, 78918, 80127, 96707, 97638],
         271: [56271],
         407: [24407],
         456: [14456],
         564: [17564],
         963: [79510, 92764]
     }, x.f.consumes = (e, r) => {
         x.o(O, e) && O[e].forEach((e => {
```

### Comparing `jupyter_ai-0.8.0/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-0.9.0/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/schema/plugin.json` & `jupyter_ai-0.9.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/chat_handler.ts` & `jupyter_ai-0.9.0/src/chat_handler.ts`

 * *Files 3% similar despite different names*

```diff
@@ -10,34 +10,33 @@
    * The server settings used to make API requests.
    */
   readonly serverSettings: ServerConnection.ISettings;
 
   /**
    * ID of the connection. Requires `await initialize()`.
    */
-  id: string = '';
+  id = '';
 
   /**
    * Create a new chat handler.
    */
   constructor(options: AiService.IOptions = {}) {
     this.serverSettings =
       options.serverSettings ?? ServerConnection.makeSettings();
   }
 
   /**
    * Initializes the WebSocket connection to the Chat backend. Promise is
    * resolved when server acknowledges connection and sends the client ID. This
    * must be awaited before calling any other method.
    */
-  public async initialize() {
+  public async initialize(): Promise<void> {
     await this._initialize();
   }
 
-
   /**
    * Sends a message across the WebSocket. Promise resolves to the message ID
    * when the server sends the same message back, acknowledging receipt.
    */
   public sendMessage(message: AiService.ChatRequest): Promise<string> {
     return new Promise(resolve => {
       this._socket?.send(JSON.stringify(message));
@@ -137,52 +136,52 @@
    */
   private _replyForResolverDict: Record<
     string,
     (value: AiService.AgentChatMessage) => void
   > = {};
 
   private _onClose(e: CloseEvent, reject: any) {
-    reject(new Error("Chat UI websocket disconnected"))
-    console.error("Chat UI websocket disconnected")
+    reject(new Error('Chat UI websocket disconnected'));
+    console.error('Chat UI websocket disconnected');
     // only attempt re-connect if there was an abnormal closure
     // WebSocket status codes defined in RFC 6455: https://www.rfc-editor.org/rfc/rfc6455.html#section-7.4.1
     if (e.code === 1006) {
-      const delaySeconds = 1
-      console.info(`Will try to reconnect in ${delaySeconds} s.`)
+      const delaySeconds = 1;
+      console.info(`Will try to reconnect in ${delaySeconds} s.`);
       setTimeout(async () => await this._initialize(), delaySeconds * 1000);
     }
   }
 
   private _initialize(): Promise<void> {
     return new Promise<void>((resolve, reject) => {
       if (this.isDisposed) {
         return;
       }
-      console.log("Creating a new websocket connection for chat...");
+      console.log('Creating a new websocket connection for chat...');
       const { token, WebSocket, wsUrl } = this.serverSettings;
       const url =
         URLExt.join(wsUrl, CHAT_SERVICE_URL) +
         (token ? `?token=${encodeURIComponent(token)}` : '');
-      
-        const socket = (this._socket = new WebSocket(url));
-        socket.onclose = (e) => this._onClose(e, reject);
-        socket.onerror = (e) => reject(e);
-        socket.onmessage = msg =>
-          msg.data && this._onMessage(JSON.parse(msg.data));
-        
-        const listenForConnection = (message: AiService.Message) => {
-          if (message.type !== 'connection') {
-            return;
-          }
-          this.id = message.client_id;
-          resolve();
-          this.removeListener(listenForConnection);
-        };
-  
-        this.addListener(listenForConnection);
+
+      const socket = (this._socket = new WebSocket(url));
+      socket.onclose = e => this._onClose(e, reject);
+      socket.onerror = e => reject(e);
+      socket.onmessage = msg =>
+        msg.data && this._onMessage(JSON.parse(msg.data));
+
+      const listenForConnection = (message: AiService.Message) => {
+        if (message.type !== 'connection') {
+          return;
+        }
+        this.id = message.client_id;
+        resolve();
+        this.removeListener(listenForConnection);
+      };
+
+      this.addListener(listenForConnection);
     });
   }
 
   private _isDisposed = false;
   private _socket: WebSocket | null = null;
   private _listeners: ((msg: any) => void)[] = [];
 }
```

### Comparing `jupyter_ai-0.8.0/src/handler.ts` & `jupyter_ai-0.9.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/icons.ts` & `jupyter_ai-0.9.0/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/index.ts` & `jupyter_ai-0.9.0/src/index.ts`

 * *Files 8% similar despite different names*

```diff
@@ -32,30 +32,31 @@
      */
     const selectionWatcher = new SelectionWatcher(app.shell);
 
     /**
      * Initialize chat handler, open WS connection
      */
     const chatHandler = new ChatHandler();
-    
+
     let chatWidget: ReactWidget | null = null;
     try {
       await chatHandler.initialize();
-      chatWidget = buildChatSidebar(selectionWatcher, chatHandler, globalAwareness);
+      chatWidget = buildChatSidebar(
+        selectionWatcher,
+        chatHandler,
+        globalAwareness
+      );
     } catch (e) {
-      chatWidget = buildErrorWidget()
+      chatWidget = buildErrorWidget();
     }
-   
+
     /**
      * Add Chat widget to right sidebar
      */
-    app.shell.add(
-      chatWidget,
-      'left', { rank: 2000 }
-    );
+    app.shell.add(chatWidget, 'left', { rank: 2000 });
 
     if (restorer) {
       restorer.add(chatWidget, 'jupyter-ai-chat');
     }
   }
 };
```

### Comparing `jupyter_ai-0.8.0/src/inserter.ts` & `jupyter_ai-0.9.0/src/inserter.ts`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 };
 
 /**
  * Function that handles the insertion of Prompt API output into the
  * active document. This function expects that a command with an id
  * of `ai:insert-<insertion-mode>` is registered, context is passed
  * through to the command for handling insertion. See `InsertionContext`
- * for more info. 
- * 
+ * for more info.
+ *
  * @param app - Jupyter front end application
  * @param context - Insertion context
  */
 export async function insertOutput(
   app: JupyterFrontEnd,
   context: InsertionContext
 ): Promise<boolean> {
```

### Comparing `jupyter_ai-0.8.0/src/selection-watcher.ts` & `jupyter_ai-0.9.0/src/selection-watcher.ts`

 * *Files 3% similar despite different names*

```diff
@@ -46,21 +46,27 @@
   }
 
   let cellId: string | undefined = undefined;
   if (widget.content instanceof Notebook) {
     cellId = widget.content.activeCell?.model.id;
   }
 
-  let { start, end, ...selectionObj } = editor.getSelection();
+  const selectionObj = editor.getSelection();
+  let { start, end } = selectionObj;
   const startOffset = editor.getOffsetAt(start);
   const endOffset = editor.getOffsetAt(end);
   const text = editor.model.sharedModel
     .getSource()
     .substring(startOffset, endOffset);
 
+  // Do not return a Selection object if no text is selected
+  if (!text) {
+    return null;
+  }
+
   // ensure start <= end
   // required for editor.model.sharedModel.updateSource()
   if (startOffset > endOffset) {
     [start, end] = [end, start];
   }
 
   return {
@@ -101,19 +107,19 @@
     this._shell.currentChanged.connect((sender, args) => {
       this._mainAreaWidget = args.newValue;
     });
 
     setInterval(this._poll.bind(this), 200);
   }
 
-  get selectionChanged() {
+  get selectionChanged(): Signal<this, Selection | null> {
     return this._selectionChanged;
   }
 
-  replaceSelection(selection: Selection) {
+  replaceSelection(selection: Selection): void {
     // unfortunately shell.currentWidget doesn't update synchronously after
     // shell.activateById(), which is why we have to get a reference to the
     // widget manually.
     const widget = find(
       this._shell.widgets(),
       widget => widget.id === selection.widgetId
     );
@@ -145,15 +151,15 @@
     );
     const newPosition = editor.getPositionAt(
       editor.getOffsetAt(selection.start) + selection.text.length
     );
     editor.setSelection({ start: newPosition, end: newPosition });
   }
 
-  protected _poll() {
+  protected _poll(): void {
     const prevSelection = this._selection;
     const currSelection = getTextSelection(this._mainAreaWidget);
 
     if (prevSelection?.text === currSelection?.text) {
       return;
     }
```

### Comparing `jupyter_ai-0.8.0/src/theme-provider.ts` & `jupyter_ai-0.9.0/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/utils.ts` & `jupyter_ai-0.9.0/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/components/chat-code-view.tsx` & `jupyter_ai-0.9.0/src/components/chat-code-view.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
   );
 }
 
 export function ChatCodeView({
   inline,
   className,
   ...props
-}: ChatCodeViewProps) {
+}: ChatCodeViewProps): JSX.Element {
   const match = /language-(\w+)/.exec(className || '');
   return inline ? (
     <ChatCodeInline {...props} />
   ) : (
     <ChatCodeBlock {...props} language={match ? match[1] : undefined} />
   );
 }
```

### Comparing `jupyter_ai-0.8.0/src/components/chat-input.tsx` & `jupyter_ai-0.9.0/src/components/chat-input.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -23,61 +23,67 @@
   replaceSelection: boolean;
   toggleReplaceSelection: () => unknown;
   sendWithShiftEnter: boolean;
   sx?: SxProps<Theme>;
 };
 
 export function ChatInput(props: ChatInputProps): JSX.Element {
-  
   function handleKeyDown(event: React.KeyboardEvent<HTMLInputElement>) {
-    if (event.key === 'Enter' && (
-      (props.sendWithShiftEnter && event.shiftKey)
-      || (!props.sendWithShiftEnter && !event.shiftKey)
-    )) {
+    if (
+      event.key === 'Enter' &&
+      ((props.sendWithShiftEnter && event.shiftKey) ||
+        (!props.sendWithShiftEnter && !event.shiftKey))
+    ) {
       props.onSend();
       event.stopPropagation();
       event.preventDefault();
     }
   }
 
   // Set the helper text based on whether Shift+Enter is used for sending.
-  const helperText = props.sendWithShiftEnter
-    ? <span>Press <b>Shift</b>+<b>Enter</b> to send message</span>
-    : <span>Press <b>Shift</b>+<b>Enter</b> to add a new line</span>;
+  const helperText = props.sendWithShiftEnter ? (
+    <span>
+      Press <b>Shift</b>+<b>Enter</b> to send message
+    </span>
+  ) : (
+    <span>
+      Press <b>Shift</b>+<b>Enter</b> to add a new line
+    </span>
+  );
 
   return (
     <Box sx={props.sx}>
-      <Box sx={{ display: 'flex'}}>
+      <Box sx={{ display: 'flex' }}>
         <TextField
           value={props.value}
           onChange={e => props.onChange(e.target.value)}
           fullWidth
           variant="outlined"
           multiline
           onKeyDown={handleKeyDown}
-          placeholder='Ask Jupyternaut anything'
+          placeholder="Ask Jupyternaut anything"
           InputProps={{
             endAdornment: (
-               <InputAdornment position="end">
-                  <IconButton
-                    size="small"
-                    color="primary"
-                    onClick={props.onSend}
-                    disabled={!props.value.trim().length}
-                    title='Send message (SHIFT+ENTER)'
-                  >
-                    <SendIcon />
-                  </IconButton>
-               </InputAdornment>
+              <InputAdornment position="end">
+                <IconButton
+                  size="small"
+                  color="primary"
+                  onClick={props.onSend}
+                  disabled={!props.value.trim().length}
+                  title="Send message (SHIFT+ENTER)"
+                >
+                  <SendIcon />
+                </IconButton>
+              </InputAdornment>
             )
-         }}
-         FormHelperTextProps={{
-          sx: {marginLeft: 'auto', marginRight: 0}
-         }}
-         helperText={props.value.length > 2 ? helperText : ' '}
+          }}
+          FormHelperTextProps={{
+            sx: { marginLeft: 'auto', marginRight: 0 }
+          }}
+          helperText={props.value.length > 2 ? helperText : ' '}
         />
       </Box>
       {props.hasSelection && (
         <FormGroup sx={{ display: 'flex', flexDirection: 'row' }}>
           <FormControlLabel
             control={
               <Checkbox
```

### Comparing `jupyter_ai-0.8.0/src/components/chat-messages.tsx` & `jupyter_ai-0.9.0/src/components/chat-messages.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 type ChatMessageHeaderProps = {
   message: AiService.ChatMessage;
   timestamp: string;
   sx?: SxProps<Theme>;
 };
 
-export function ChatMessageHeader(props: ChatMessageHeaderProps) {
+export function ChatMessageHeader(props: ChatMessageHeaderProps): JSX.Element {
   const collaborators = useCollaboratorsContext();
 
   const sharedStyles: SxProps<Theme> = {
     height: '24px',
     width: '24px'
   };
 
@@ -97,33 +97,32 @@
           {props.timestamp}
         </Typography>
       </Box>
     </Box>
   );
 }
 
-export function ChatMessages(props: ChatMessagesProps) {
+export function ChatMessages(props: ChatMessagesProps): JSX.Element {
   const [timestamps, setTimestamps] = useState<Record<string, string>>({});
 
   /**
    * Effect: update cached timestamp strings upon receiving a new message.
    */
   useEffect(() => {
     const newTimestamps: Record<string, string> = { ...timestamps };
-    let timestampAdded: boolean = false;
+    let timestampAdded = false;
 
     for (const message of props.messages) {
       if (!(message.id in newTimestamps)) {
         // Use the browser's default locale
-        newTimestamps[message.id] =
-          new Date(message.time * 1000) // Convert message time to milliseconds
-            .toLocaleTimeString([], {
-              hour: 'numeric', // Avoid leading zero for hours; we don't want "03:15 PM"
-              minute: '2-digit'
-            });
+        newTimestamps[message.id] = new Date(message.time * 1000) // Convert message time to milliseconds
+          .toLocaleTimeString([], {
+            hour: 'numeric', // Avoid leading zero for hours; we don't want "03:15 PM"
+            minute: '2-digit'
+          });
 
         timestampAdded = true;
       }
     }
     if (timestampAdded) {
       setTimestamps(newTimestamps);
     }
```

### Comparing `jupyter_ai-0.8.0/src/components/chat-settings.tsx` & `jupyter_ai-0.9.0/src/components/chat-settings.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
  * - `config` is the configuration last fetched from the backend. `inputConfig`
  * is the editable copy of that object that stores all user input state.
  *
  * - `inputConfig.model_provider_id` reflects the global model ID only if the
  * provider is not a registry provider. Otherwise, it is set to
  * `<provider-id>:*`.
  */
-export function ChatSettings() {
+export function ChatSettings(): JSX.Element {
   const [state, setState] = useState<ChatSettingsState>(
     ChatSettingsState.Loading
   );
   // error message from initial fetch
   const [fetchEmsg, setFetchEmsg] = useState<string>();
 
   // state fetched on initial render
@@ -285,15 +285,16 @@
   }
 
   return (
     <Box
       sx={{
         padding: 4,
         boxSizing: 'border-box',
-        '& > .MuiAlert-root': { marginBottom: 2 }
+        '& > .MuiAlert-root': { marginBottom: 2 },
+        overflowY: 'auto'
       }}
     >
       {state === ChatSettingsState.SubmitError && (
         <Alert severity="error">
           {saveEmsg
             ? `An error occurred. Error details:\n\n${saveEmsg}`
             : 'An unknown error occurred. Check the console for more details.'}
```

### Comparing `jupyter_ai-0.8.0/src/components/chat.tsx` & `jupyter_ai-0.9.0/src/components/chat.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 import { SelectionWatcher } from '../selection-watcher';
 import { ChatHandler } from '../chat_handler';
 import { CollaboratorsContextProvider } from '../contexts/collaborators-context';
 import { ScrollContainer } from './scroll-container';
 
 type ChatBodyProps = {
   chatHandler: ChatHandler;
-  setChatView: (view: ChatView) => void
+  setChatView: (view: ChatView) => void;
 };
 
-function ChatBody({ chatHandler, setChatView: chatViewHandler }: ChatBodyProps): JSX.Element {
+function ChatBody({
+  chatHandler,
+  setChatView: chatViewHandler
+}: ChatBodyProps): JSX.Element {
   const [messages, setMessages] = useState<AiService.ChatMessage[]>([]);
   const [showWelcomeMessage, setShowWelcomeMessage] = useState<boolean>(false);
   const [includeSelection, setIncludeSelection] = useState(true);
   const [replaceSelection, setReplaceSelection] = useState(false);
   const [input, setInput] = useState('');
   const [selection, replaceSelectionFn] = useSelectionContext();
   const [sendWithShiftEnter, setSendWithShiftEnter] = useState(true);
@@ -102,17 +105,17 @@
         ...(cellId && { cellId }),
         text: reply.body
       });
     }
   };
 
   const openSettingsView = () => {
-    setShowWelcomeMessage(false)
-    chatViewHandler(ChatView.Settings)
-  }
+    setShowWelcomeMessage(false);
+    chatViewHandler(ChatView.Settings);
+  };
 
   if (showWelcomeMessage) {
     return (
       <Box
         sx={{
           padding: 4,
           display: 'flex',
@@ -123,21 +126,21 @@
       >
         <Stack spacing={4}>
           <p>
             Welcome to Jupyter AI! To get started, please select a language
             model to chat with from the settings panel. You will also likely
             need to provide API credentials, so be sure to have those handy.
           </p>
-          <Button 
-            variant="contained" 
-            startIcon={<SettingsIcon />} 
+          <Button
+            variant="contained"
+            startIcon={<SettingsIcon />}
             size={'large'}
             onClick={() => openSettingsView()}
-            >
-              Start Here
+          >
+            Start Here
           </Button>
         </Stack>
       </Box>
     );
   }
 
   return (
@@ -171,23 +174,23 @@
   );
 }
 
 export type ChatProps = {
   selectionWatcher: SelectionWatcher;
   chatHandler: ChatHandler;
   globalAwareness: Awareness | null;
-  chatView?: ChatView
+  chatView?: ChatView;
 };
 
 enum ChatView {
   Chat,
   Settings
 }
 
-export function Chat(props: ChatProps) {
+export function Chat(props: ChatProps): JSX.Element {
   const [view, setView] = useState<ChatView>(props.chatView || ChatView.Chat);
 
   return (
     <JlThemeProvider>
       <SelectionContextProvider selectionWatcher={props.selectionWatcher}>
         <CollaboratorsContextProvider globalAwareness={props.globalAwareness}>
           <Box
@@ -217,15 +220,15 @@
                 </IconButton>
               ) : (
                 <Box />
               )}
             </Box>
             {/* body */}
             {view === ChatView.Chat && (
-              <ChatBody chatHandler={props.chatHandler} setChatView={setView}/>
+              <ChatBody chatHandler={props.chatHandler} setChatView={setView} />
             )}
             {view === ChatView.Settings && <ChatSettings />}
           </Box>
         </CollaboratorsContextProvider>
       </SelectionContextProvider>
     </JlThemeProvider>
   );
```

### Comparing `jupyter_ai-0.8.0/src/components/expandable-text-field.tsx` & `jupyter_ai-0.9.0/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/src/components/jl-theme-provider.tsx` & `jupyter_ai-0.9.0/src/components/jl-theme-provider.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import React, { useState, useEffect } from 'react';
 
 import { Theme, ThemeProvider, createTheme } from '@mui/material/styles';
 import { getJupyterLabTheme } from '../theme-provider';
 
-export function JlThemeProvider(props: { children: React.ReactNode }) {
+export function JlThemeProvider(props: {
+  children: React.ReactNode;
+}): JSX.Element {
   const [theme, setTheme] = useState<Theme>(createTheme());
 
   useEffect(() => {
     async function setJlTheme() {
       setTheme(await getJupyterLabTheme());
     }
     setJlTheme();
```

### Comparing `jupyter_ai-0.8.0/src/components/scroll-container.tsx` & `jupyter_ai-0.9.0/src/components/scroll-container.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,28 @@
  *
  * Currently only works for Chrome and Firefox due to reliance on
  * `overflow-anchor`.
  *
  * **References**
  * - https://css-tricks.com/books/greatest-css-tricks/pin-scrolling-to-bottom/
  */
-export function ScrollContainer(props: ScrollContainerProps) {
+export function ScrollContainer(props: ScrollContainerProps): JSX.Element {
   const id = useMemo(
     () => 'jupyter-ai-scroll-container-' + Date.now().toString(),
     []
   );
 
   /**
    * Effect: Scroll the container to the bottom as soon as it is visible.
    */
   useEffect(() => {
     const el = document.querySelector<HTMLElement>(`#${id}`);
-    if (!el) return;
+    if (!el) {
+      return;
+    }
 
     const observer = new IntersectionObserver(
       entries => {
         entries.forEach(entry => {
           if (entry.isIntersecting) {
             el.scroll({ top: 999999999 });
           }
```

### Comparing `jupyter_ai-0.8.0/src/components/select.tsx` & `jupyter_ai-0.9.0/src/components/select.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  * prepends an input label derived from `props.label`.
  *
  * - limits max height of menu
  *
  * - handles `null` values by coercing them to the string `'null'`. The
  * corresponding `MenuItem` should have the value `'null'`.
  */
-export function Select(props: SelectProps) {
+export function Select(props: SelectProps): JSX.Element {
   return (
     <FormControl fullWidth>
       <InputLabel>{props.label}</InputLabel>
       <MuiSelect
         {...props}
         value={props.value === null ? 'null' : props.value}
         label={props.label}
```

### Comparing `jupyter_ai-0.8.0/src/components/settings/model-fields.tsx` & `jupyter_ai-0.9.0/src/components/settings/model-fields.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
   return <></>;
 }
 
 export type ModelFieldsProps = Omit<ModelFieldProps, 'field'> & {
   fields?: AiService.Field[];
 };
 
-export function ModelFields(props: ModelFieldsProps) {
+export function ModelFields(props: ModelFieldsProps): JSX.Element | null {
   if (!props.fields?.length) {
     return null;
   }
 
   return (
     <>
       {props.fields.map((field, idx) => (
```

### Comparing `jupyter_ai-0.8.0/src/contexts/collaborators-context.tsx` & `jupyter_ai-0.9.0/src/contexts/collaborators-context.tsx`

 * *Files 18% similar despite different names*

```diff
@@ -7,28 +7,30 @@
   Record<string, AiService.Collaborator>
 >({});
 
 /**
  * Returns a dictionary mapping each collaborator's username to their associated
  * Collaborator object.
  */
+// eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
 export function useCollaboratorsContext() {
   return useContext(CollaboratorsContext);
 }
 
 type GlobalAwarenessStates = Map<
   number,
   { current: string; user: AiService.Collaborator }
 >;
 
 type CollaboratorsContextProviderProps = {
   globalAwareness: Awareness | null;
   children: JSX.Element;
 };
 
+// eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
 export function CollaboratorsContextProvider({
   globalAwareness,
   children
 }: CollaboratorsContextProviderProps) {
   const [collaborators, setCollaborators] = useState<
     Record<string, AiService.Collaborator>
   >({});
```

### Comparing `jupyter_ai-0.8.0/src/contexts/selection-context.tsx` & `jupyter_ai-0.9.0/src/contexts/selection-context.tsx`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 >([
   null,
   () => {
     /* noop */
   }
 ]);
 
+// eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
 export function useSelectionContext() {
   return useContext(SelectionContext);
 }
 
 type SelectionContextProviderProps = {
   selectionWatcher: SelectionWatcher;
   children: React.ReactNode;
 };
 
+// eslint-disable-next-line @typescript-eslint/explicit-module-boundary-types
 export function SelectionContextProvider({
   selectionWatcher,
   children
 }: SelectionContextProviderProps) {
   const [selection, setSelection] = useState<Selection | null>(null);
 
   /**
```

### Comparing `jupyter_ai-0.8.0/src/widgets/chat-error.tsx` & `jupyter_ai-0.9.0/src/widgets/chat-error.tsx`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import React from 'react';
 import { ReactWidget } from '@jupyterlab/apputils';
 
 import { chatIcon } from '../icons';
 import { Alert, Box } from '@mui/material';
 import { JlThemeProvider } from '../components/jl-theme-provider';
 
-export function buildErrorWidget() {
-    const ErrorWidget = ReactWidget.create(
-        <JlThemeProvider>
-            <Box
-                sx={{
-                    width: '100%',
-                    height: '100%',
-                    boxSizing: 'border-box',
-                    background: 'var(--jp-layout-color0)',
-                    display: 'flex',
-                    flexDirection: 'column'
-                }}
-            >
-                <Box sx={{ padding: 4 }}>
-                    <Alert severity="error">
-                        There seems to be a problem with the Chat backend, please look at the
-                        JupyterLab server logs or contact your administrator to correct this
-                        problem.
-                    </Alert>
-                </Box>
-            </Box>
-        </JlThemeProvider>
-    );
-    ErrorWidget.id = 'jupyter-ai::chat';
-    ErrorWidget.title.icon = chatIcon;
-    ErrorWidget.title.caption = 'Jupyter AI Chat'; // TODO: i18n
-    
-    return ErrorWidget
-}
+export function buildErrorWidget(): ReactWidget {
+  const ErrorWidget = ReactWidget.create(
+    <JlThemeProvider>
+      <Box
+        sx={{
+          width: '100%',
+          height: '100%',
+          boxSizing: 'border-box',
+          background: 'var(--jp-layout-color0)',
+          display: 'flex',
+          flexDirection: 'column'
+        }}
+      >
+        <Box sx={{ padding: 4 }}>
+          <Alert severity="error">
+            There seems to be a problem with the Chat backend, please look at
+            the JupyterLab server logs or contact your administrator to correct
+            this problem.
+          </Alert>
+        </Box>
+      </Box>
+    </JlThemeProvider>
+  );
+  ErrorWidget.id = 'jupyter-ai::chat';
+  ErrorWidget.title.icon = chatIcon;
+  ErrorWidget.title.caption = 'Jupyter AI Chat'; // TODO: i18n
 
+  return ErrorWidget;
+}
```

### Comparing `jupyter_ai-0.8.0/src/widgets/chat-sidebar.tsx` & `jupyter_ai-0.9.0/src/widgets/chat-sidebar.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import { SelectionWatcher } from '../selection-watcher';
 import { ChatHandler } from '../chat_handler';
 
 export function buildChatSidebar(
   selectionWatcher: SelectionWatcher,
   chatHandler: ChatHandler,
   globalAwareness: Awareness | null
-) {
+): ReactWidget {
   const ChatWidget = ReactWidget.create(
     <Chat
       selectionWatcher={selectionWatcher}
       chatHandler={chatHandler}
       globalAwareness={globalAwareness}
     />
   );
```

### Comparing `jupyter_ai-0.8.0/style/icons/jupyternaut.svg` & `jupyter_ai-0.9.0/style/icons/jupyternaut.svg`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 000007f0: 2020 203c 636c 6970 5061 7468 2069 643d     <clipPath id=
 00000800: 2263 6c69 7030 5f30 5f32 3335 3622 3e0a  "clip0_0_2356">.
 00000810: 2020 2020 2020 2020 2020 2020 3c72 6563              <rec
 00000820: 7420 7769 6474 683d 2233 3822 2068 6569  t width="38" hei
 00000830: 6768 743d 2233 3822 2066 696c 6c3d 2277  ght="38" fill="w
 00000840: 6869 7465 2220 2f3e 0a20 2020 2020 2020  hite" />.       
 00000850: 203c 2f63 6c69 7050 6174 683e 0a20 2020   </clipPath>.   
-00000860: 203c 2f64 6566 733e 0a3c 2f73 7667 3e     </defs>.</svg>
+00000860: 203c 2f64 6566 733e 0a3c 2f73 7667 3e0a   </defs>.</svg>.
```

### Comparing `jupyter_ai-0.8.0/ui-tests/README.md` & `jupyter_ai-0.9.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-0.9.0/ui-tests/jupyter_server_test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from tempfile import mkdtemp
 
 c.ServerApp.port = 8888
 c.ServerApp.port_retries = 0
 c.ServerApp.open_browser = False
 
-c.ServerApp.root_dir = mkdtemp(prefix='galata-test-')
+c.ServerApp.root_dir = mkdtemp(prefix="galata-test-")
 c.ServerApp.token = ""
 c.ServerApp.password = ""
 c.ServerApp.disable_check_xsrf = True
 c.LabApp.expose_app_in_browser = True
 
 # Uncomment to set server log level to debug level
 # c.ServerApp.log_level = "DEBUG"
```

### Comparing `jupyter_ai-0.8.0/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-0.9.0/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/.gitignore` & `jupyter_ai-0.9.0/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 # OSX files
 .DS_Store
 
 # vscode
 .vscode
 
 # Coverage reports
-coverage/*
+coverage/*
```

### Comparing `jupyter_ai-0.8.0/LICENSE` & `jupyter_ai-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-0.8.0/README.md` & `jupyter_ai-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     $ conda create -n jupyter-ai python=3.10
     $ conda activate jupyter-ai
     $ pip install jupyter_ai
 
 If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
 
-    $ pip uninstall grpcio; conda install grpcio 
+    $ pip uninstall grpcio; conda install grpcio
 
 ## Uninstall
 
 To remove the extension, execute:
 
     $ pip uninstall jupyter_ai
```

### Comparing `jupyter_ai-0.8.0/pyproject.toml` & `jupyter_ai-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -49,22 +49,20 @@
     "coverage",
     "pytest",
     "pytest-asyncio",
     "pytest-cov",
     "pytest-tornasync"
 ]
 
+dev = [
+    "jupyter_ai_magics[dev]"
+]
+
 all = [
-    "ai21",
-    "anthropic",
-    "cohere",
-    "huggingface_hub",
-    "ipywidgets",
-    "openai",
-    "boto3"
+    "jupyter_ai_magics[all]"
 ]
 
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
```

### Comparing `jupyter_ai-0.8.0/PKG-INFO` & `jupyter_ai-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 0.8.0
+Version: 0.9.0
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -57,21 +57,17 @@
 Requires-Dist: langchain==0.0.159
 Requires-Dist: openai~=0.26
 Requires-Dist: pydantic
 Requires-Dist: ray~=2.4.0
 Requires-Dist: tiktoken
 Requires-Dist: typing-extensions==4.5.0
 Provides-Extra: all
-Requires-Dist: ai21; extra == 'all'
-Requires-Dist: anthropic; extra == 'all'
-Requires-Dist: boto3; extra == 'all'
-Requires-Dist: cohere; extra == 'all'
-Requires-Dist: huggingface-hub; extra == 'all'
-Requires-Dist: ipywidgets; extra == 'all'
-Requires-Dist: openai; extra == 'all'
+Requires-Dist: jupyter-ai-magics[all]; extra == 'all'
+Provides-Extra: dev
+Requires-Dist: jupyter-ai-magics[dev]; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: jupyter-server[test]<3,>=1.6; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-tornasync; extra == 'test'
@@ -109,15 +105,15 @@
 
     $ conda create -n jupyter-ai python=3.10
     $ conda activate jupyter-ai
     $ pip install jupyter_ai
 
 If you are using an Apple Silicon-based Mac (M1, M1 Pro, M2, etc.), you need to uninstall the `pip` provided version of `grpcio` and install the version provided by `conda` instead.
 
-    $ pip uninstall grpcio; conda install grpcio 
+    $ pip uninstall grpcio; conda install grpcio
 
 ## Uninstall
 
 To remove the extension, execute:
 
     $ pip uninstall jupyter_ai
```

