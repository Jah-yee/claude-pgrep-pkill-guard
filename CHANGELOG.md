# Changelog

## [2.0.0](https://github.com/rvenutolo/claude-pgrep-pkill-guard/compare/v1.1.0...v2.0.0) (2026-10-08)


### ⚠ BREAKING CHANGES

* raise the hook's bash floor to 4.4 ([#237](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/237))
* the guard now requires bash 4.4 or newer. On bash 4.3 it reports itself INACTIVE for every command instead of guarding. Stock macOS bash 3.2 was already below the floor; Homebrew bash and current Linux distributions ship 5.x.

### Features

* accept a fixture dir in check-executable-bit ([ed648a5](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ed648a50c8c8cfcc7803de8bdc6bd33fc49f6006)), closes [#322](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/322)
* fail check-executable-bit on a row that matches nothing ([f138cfd](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/f138cfdbe77ffe6c6369228a4591c0fd31edab94)), closes [#322](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/322)
* fail check-executable-bit on a row that matches nothing ([#326](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/326)) ([fa93a1b](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/fa93a1b887ff3573e358057d1b5593475f8c5586))
* raise the hook's bash floor to 4.4 ([eb6f39e](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/eb6f39e29250cf5cfb7538316ac7a9a6bc9ed9cf)), closes [#209](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/209)
* raise the hook's bash floor to 4.4 ([#237](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/237)) ([9d8601f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/9d8601f5b4e95efec6fccc333e6534f83b74a896))
* reject surplus arguments in optional-argument gates ([23061f3](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/23061f30735654b5d54103f49a6192e32c0b18df)), closes [#216](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/216)
* reject surplus arguments in optional-argument gates ([#241](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/241)) ([3e970f3](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3e970f30bfdf203e86669aa1bf70e0146262a337))


### Bug Fixes

* accept only an exact main "$@" as the last statement ([14fbfc5](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/14fbfc536ffbd7a38d669e75e2cc8b7418a67d4a))
* blame multi-line quoted strings, not heredocs, in the kcov caveat ([66508a0](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/66508a06dd0bf61f139dcc894f9de0610743b2ce)), closes [#275](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/275)
* build the one-true-awk shim once for a repeated --awk=bwk ([ea783f3](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ea783f3d2cb048ceb36dbe2c33f0873dd15cff87))
* declare three leaking function variables local ([23c1eaa](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/23c1eaa7a2019cc4e030ce0f995a6f7919f60bed)), closes [#222](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/222)
* declare three leaking function variables local ([#256](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/256)) ([3f4ec1e](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3f4ec1eed9eec9a765288a30d8ce193f9196537a))
* drop issue numbers inherited from the dotfiles repo ([aacef4f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/aacef4fffbc3d2d4a7d8fe38d9f74345f71d8c0b)), closes [#208](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/208)
* drop issue numbers inherited from the dotfiles repo ([#236](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/236)) ([8670539](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/8670539e2494f3c7ee57567d448a4cd0d4e91e68))
* drop the wrapper pipe carry when its own stdin is redirected ([2a3106e](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/2a3106e56dd1692e2bcf020607855e8f9f8416c9)), closes [#361](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/361)
* drop the wrapper pipe carry when its own stdin is redirected ([#394](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/394)) ([161e8c6](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/161e8c6fbfc711af31cd84ed2ce4f661ef608909))
* fail run-lint-checks on an empty Markdown file list ([c396f96](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c396f96e39589f44e79fecca2c251dfffc5e7419))
* fail run-lint-checks on an empty Markdown file list ([#375](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/375)) ([61cde21](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/61cde21002a15e00c7a5c3e85e11364d246e3e93))
* guard host-bash scripts against bash older than 4.4 ([#233](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/233)) ([5823f95](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/5823f95ea3e3b00944ae70f9346c3a5939c5293a))
* join an unquoted heredoc body line ending in a backslash ([f4b6f69](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/f4b6f695abec738b3bc24101631a7baf16081820)), closes [#362](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/362)
* join an unquoted heredoc body line ending in a backslash ([#387](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/387)) ([9debe7b](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/9debe7b5381839730582cbdab3ded31f41975b91))
* keep a prefix flag's value out of the wrapper pipe carry ([1fba663](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/1fba6639e640776dd0d1671473181fa2b37a96ff)), closes [#380](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/380)
* keep a prefix flag's value out of the wrapper pipe carry ([#391](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/391)) ([3f6f74d](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3f6f74dd8e5499e6a316540fcd53bc11ac4d8ace))
* keep a wrapper open across a dup or clobber redirection ([9334fb8](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/9334fb808963742b1f08ff5288f5ede41e45773c)), closes [#392](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/392)
* keep a wrapper open across a dup or clobber redirection ([#399](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/399)) ([ff988b4](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ff988b40a9609f0203bc668641bc848f38580dd5))
* keep lint config out of archives and build the awk shim once ([#381](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/381)) ([feb7748](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/feb77487af1a63917cb325f7e6408e9e67f29dcd))
* keep prettier and shellcheck config out of release archives ([e010704](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/e010704d1e9413b43145daf55e674817e03aa504))
* name a missing bench report by its relative path ([cd19b97](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/cd19b97752b8f0ad5691135b64cfa5d986fddec4))
* quote EXIT-trap temp paths with printf %q ([#235](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/235)) ([9fa14d1](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/9fa14d101e3d0d80fa2053ed33dfd3215c23443d))
* raise run-tests and in-devshell bash guards to 4.4 ([#234](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/234)) ([403b73d](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/403b73db173d0ceedeb692fd0cd6ebef10623885))
* reject a malformed --report in run-all-checks ([e8a1541](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/e8a1541c6f7f5f20e352ecef859c1ad61896b8ab)), closes [#272](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/272)
* reject a malformed --report in run-all-checks ([#287](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/287)) ([b8572de](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/b8572def572720c60ff3906f5a44ddd37aecfa06))
* reject an unterminated one-line shebang in bats files ([25796a9](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/25796a93c1b2ae931e2d5e1ba3dcb04098b61b57)), closes [#305](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/305)
* reject an unterminated one-line shebang in bats files ([#315](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/315)) ([2fd3f60](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/2fd3f60f1b8a345d9dff087e363ab7da7d041540))
* skip a redirection in the backward walk from a pgrep ([23b2e78](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/23b2e780386f5184ff75e4192f2ac4b4996bd479))
* skip a redirection while hunting for the command word ([1cefa83](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/1cefa8389bf7127a3d2327a9add64422b6e7e8fa)), closes [#397](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/397)
* skip a redirection while hunting for the command word ([#403](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/403)) ([83b82fd](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/83b82fdcff6f9090950743cdb7eb4ccab36489b8))
* skip the target of any redirection operator in pattern_operand ([8e12815](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/8e128158a7626f0545fee75d73d56445abe25eab))
* skip the target of any redirection operator in pattern_operand ([#388](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/388)) ([c149d0a](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c149d0a2e0987f7c3846f8e4480beec5f3e4a60a))
* split a word at a redirection operator in the scanner ([3577f89](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3577f89d6a8035f40eb6d116fa54645b1b7c93cd))
* split a word at a redirection operator in the scanner ([#401](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/401)) ([446765c](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/446765c228f21296d8405acc23f98a8760c8b78c))
* split ls-files --stage on the tab in check-executable-bit ([b5dd798](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/b5dd7981d6fedd1732c7d3f4c52b87a95ea3cd66)), closes [#322](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/322)


### Performance Improvements

* scan files concurrently in the bash style gate ([57ef871](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/57ef871f3767e90c3f4e2bb7d2762c1270e11306))

## [1.1.0](https://github.com/rvenutolo/claude-pgrep-pkill-guard/compare/v1.0.0...v1.1.0) (2026-09-10)

### Features

- add --help and --version to the guard's entry script ([dd72a4c](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/dd72a4c732e46d4cfdc5b06cdfb694b56310ea8b)), closes [#34](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/34)
- add --help and --version to the guard's entry script ([#60](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/60)) ([0a7ee36](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/0a7ee36f437f0381ecdc06b9b6d891e7eef9b96e))
- add a just fix recipe that runs every auto-fixer ([69492d8](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/69492d82e04dd7c0d3a4c0742e9ce70c03e525af))
- add a social preview card and the script that builds it ([48d34fb](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/48d34fb5bf7b524c0036d071d06e101acfc444b3)), closes [#35](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/35)
- add a social preview card and the script that builds it ([#66](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/66)) ([0454908](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/04549084b4c48fb5cf5842bc9b6cedc0bab43ebd))
- record machine state in benchmark provenance and regenerate ([#119](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/119)) ([58573d7](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/58573d7219fdb5a10384353ab958f015bfd55db3))
- record machine state in the benchmark provenance table ([ffc95d6](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ffc95d62fbae45a382ad2c78195e18c2d34b859d))

### Bug Fixes

- create the release formatting commit through the API ([83cd6ce](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/83cd6cea53e70feff6c5387158cd21336b29f331)), closes [#70](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/70)
- create the release formatting commit through the API ([#95](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/95)) ([a32b475](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/a32b475b3edccd2a26d1f7889b5946791d696428)), closes [#70](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/70)
- create the report directory with a POSIX mkdir -p ([56ece02](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/56ece0206ffb8ad458d3dcfa1de8a03d68f3d228))
- exclude renovate's Handlebars template from the link check ([c357f34](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c357f340272a84f0152ee5b35a29853d6c13e32f))
- exclude the changelog release compare link from the link check ([#99](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/99)) ([720137a](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/720137af01397d3e9893e083d739399b0541ec4f)), closes [#98](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/98)
- exclude the changelog's release compare link from the link check ([c416b1f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c416b1f7473f07d064c829d826c65c12f3cd42b4)), closes [#98](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/98)
- exempt the release-please version line from the bench gate ([33ba956](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/33ba9568cb5689d64079ad56b9d8cecb06c1c621))
- exempt the release-please version line from the bench gate ([#143](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/143)) ([dd8935c](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/dd8935ca2c4b6a7820f6036d01090cacbce0794c))
- guard the scanner's trailing-newline strip on empty input ([ec5f5be](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ec5f5be0c85dc97c9fea6982e9bb96bf4b9cd21a))
- make renovate's bats manager resolve, and gate the config ([#102](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/102)) ([a639e44](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/a639e4442950065c4383ad4e65ccb406efa789de))
- pass commit blobs to jq through files, not argv ([73ec72a](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/73ec72ab03be70af065168bac1733a79745df089)), closes [#94](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/94)
- pass commit payload blobs to jq through files, not argv ([#124](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/124)) ([f576fbf](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/f576fbff5238c3e04a911e7d04f624d32ac67d8b))
- pin nix in the devShell and justify packages by PATH, not by scan ([e37df97](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/e37df973f07f7b1bd5f8d893ca81a9d26b29bbfd))
- reach the enclosing if past a prefix's flags and operands ([8bfd204](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/8bfd20411f8acae0575b882ea32aaf813c1a6e7d)), closes [#132](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/132)
- refuse to report a coverage run that lost a file, and say why ([#129](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/129)) ([4db7fb1](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/4db7fb1b79619cda7b218c45b2e23b2c80511d4c))
- refuse to report a coverage run that lost a hooks file ([61484a8](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/61484a88c562fecc3eb3231559137fc4869a2a91)), closes [#128](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/128)
- resolve the bats pins with git-refs instead of github-tags ([0018fb8](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/0018fb87d548c2019efd0ef607d3b102f649e3a5)), closes [#71](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/71)
- skip the --awk=bwk cases when nawk is not one-true-awk ([4e14292](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/4e14292c9d8708ea379261dae0fc93209f7f1ba3))
- skip the devShell suite ambiently and report eval failure honestly ([988828f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/988828fe3088d62f2839b542fa0ba0002e4605e6))
- stop the ERR trap reporting a gate's own deliberate failure ([c838df7](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c838df74c9b7ac4c94eaf6e5398e50b484be081f)), closes [#43](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/43)
- stop the ERR trap reporting a gate's own deliberate failure ([#63](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/63)) ([3d63266](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3d63266ebb8dd903f99c02003bfdec62cccfcd1b))
- stop the link checker failing on prose that quotes its own patterns ([d653b51](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/d653b516b27287530f7d051f93ea47a398426b54))
- stop the release job failing when there is nothing to release ([a78fda0](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/a78fda034ff945b518f5d5bb00f15dd85165fc81)), closes [#103](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/103)
- stop the release job failing when there is nothing to release ([#104](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/104)) ([e28f2e2](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/e28f2e2ecf062b7366beb63620eb2b341d722cd6))
- stop typos rejecting the SHAs release-please writes to the changelog ([65634bd](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/65634bd92f5f28b18cbe9a88e04de6308ff2e649)), closes [#61](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/61)
- stop typos rejecting the SHAs release-please writes to the changelog ([#62](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/62)) ([1036ee1](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/1036ee1ecc5c9c93381bcdef37674c12da3f2756))
- strip any trailing newline from a staged base64 blob ([07d2be4](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/07d2be469b2f899f2c878bb4f280bd3a35d93b6e)), closes [#94](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/94)

### Performance Improvements

- **bench:** measure a typical-command cohort, not just the corpus ([21d966f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/21d966f1af10113951e373a7aef3565b8622bc20))
- **bench:** republish the per-call cost after the prefilter ([944fbc2](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/944fbc2ba01a7c0fb83e0363632d8291549e542c))
- **bench:** split the prefilter short-circuit into its own cohort ([ffe393a](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ffe393a215bf134d56c6f3d07a51a992f5219e34))
- drop the two helper spawns from the hook's fast path ([17dcd50](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/17dcd508559302c277e4616fb1f99bb2b5ae5d1c)), closes [#54](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/54)
- drop the two helper spawns from the hook's fast path ([#56](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/56)) ([281521f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/281521fa3058a53500b528056fc8e98e2c0f073a))
- micro-benchmark the hook and publish the per-call cost ([#48](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/48)) ([8ebdebc](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/8ebdebcfb841ec7ff2da550e39c8bc042bb19541))
- short-circuit the hook before the jq and awk spawns ([3abe9ce](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3abe9cefeea89e83e3621ddc9039d0f37ae4d502))
- short-circuit the hook before the jq and awk spawns ([#53](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/53)) ([39de1bf](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/39de1bf6092df4f81bdf6aab4c84eac478f0bd7a))
- split the guard so the fast path parses 152 lines, not 2203 ([6fa70a0](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/6fa70a012aee392c32b0fea2bf3022079afb0f21)), closes [#55](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/55)
- split the guard so the fast path parses 152 lines, not 2203 ([#57](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/57)) ([33ba166](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/33ba16607942084201e9f1b140daf95488d1a68f))

## 1.0.0 (2026-08-28)

### Features

- add plugin, marketplace and hook manifests ([c89bebd](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/c89bebda6ae7f95fa6544e53870a7e2dc97baa02))
- import guard hook and plugin manifests ([df27581](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/df27581c3231545ec9b739d8385ed9e3f604d4d3))
- import the pgrep/pkill guard hook and scanner ([2b8fa01](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/2b8fa01c16f2eb7dcb7c8bc7473a5e2794839b10))

### Bug Fixes

- give body_has_terminator a command-substitution scope barrier ([f845e6d](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/f845e6d6930eeec8a3f17e438981da5acbe3565b))
- give body_has_terminator a command-substitution scope barrier ([5311b34](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/5311b34554e1ae5cd42f1aa3b9a580fa26700e69)), closes [#8](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/8)
- make pgrep-scan.awk independent of RS so one-true-awk works unaided ([17cb928](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/17cb928776dcbf39e5095b03286f59bfd3d14a2b))
- make pgrep-scan.awk independent of RS so one-true-awk works unaided ([bb1c2dc](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/bb1c2dc9d2469b40554ab79d0387a251d770d8b1)), closes [#7](https://github.com/rvenutolo/claude-pgrep-pkill-guard/issues/7)
- make the guard portable and rename it ([134e939](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/134e93997b5c5c6e26c3649e2d70809079b75eb4))
- reject a pre-4.2 host bash in .ci/in-devshell ([b7c3c32](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/b7c3c3291e657617cd98f94facd95f63e5078b5f))
- report INACTIVE loudly when bash is older than 4.3 ([3e9a3dd](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/3e9a3dd737a52ad3eace051d470f17669b4a8316))
- use POSIX short flags in the guard for macOS support ([ee45d68](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/ee45d68ba99a4b9f2eb2daa364077b549512109b))
- use the security category and sync the marketplace version ([a2f54a6](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/a2f54a626b2a5d46c50fd7ab87878bc383758005))
- verify scanner integrity in-band instead of via the ERR trap ([5e3264f](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/5e3264f357cf110670a0d0868d7e99416a3075ea))

### Continuous Integration

- add release-please, commitlint and renovate ([31feb1d](https://github.com/rvenutolo/claude-pgrep-pkill-guard/commit/31feb1d796bf66dd1392cb28907f43b52a61ba1e))
