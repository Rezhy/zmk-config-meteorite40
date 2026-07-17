# Changelog

## [4.5.0](https://github.com/Rezhy/zmk-config-meteorite40/compare/v4.4.0...v4.5.0) (2026-07-17)


### Features

* move SETTING entry back to NAV+P ([51bf596](https://github.com/Rezhy/zmk-config-meteorite40/commit/51bf59645350d270d39fabf8d3e4a5d3383dced2))
* port Keyball39-style layout with US-on-JIS morphs (low profile) ([881c0ec](https://github.com/Rezhy/zmk-config-meteorite40/commit/881c0ec003a6b49d349d4358f81b770e2000445e))
* scroll on SYM layer inverted by default, Ctrl/Shift on A/Z corners ([e5c9e0f](https://github.com/Rezhy/zmk-config-meteorite40/commit/e5c9e0fb7fad71d2db624a8d49cc3742f58c9031))
* shift IME thumbs one key left, add NUM layer-tap on Q ([88b2f2d](https://github.com/Rezhy/zmk-config-meteorite40/commit/88b2f2d287efe5446fc77aef4e6a961bbddf907d))
* swap Enter and Del on the thumb row ([40e7926](https://github.com/Rezhy/zmk-config-meteorite40/commit/40e7926a0e55b3ab8871b77425f3d3a1246a3749))
* swap Tab/Space thumbs, move SETTING entry to NAV+Q ([e13243d](https://github.com/Rezhy/zmk-config-meteorite40/commit/e13243da020ea4e131aa183d48471d8d90bcf402))


### Bug Fixes

* keep empty combos node required by studio combo subsystem ([d729928](https://github.com/Rezhy/zmk-config-meteorite40/commit/d729928f449ace87427ff1b787fc24995889cae1))
* send JIS semicolon VK for Ctrl+equals shortcuts ([6900d70](https://github.com/Rezhy/zmk-config-meteorite40/commit/6900d70732ae32650c2f581e82071a73438358be))

## [4.4.0](https://github.com/iwk7273/zmk-config-meteorite40/compare/v4.3.1...v4.4.0) (2026-07-13)


### 新機能

* Mod-tap / Layer-tap の Flavor、Tapping term、Quick tap、Require prior idle を Meteorite Studio から調整できるようになりました。
* Idle timeout と Deep sleep timeout を Meteorite Studio から調整できるようになりました。
* System 設定をキーボード本体へ保存し、電源を入れ直した後も維持するようになりました。 ([#17](https://github.com/iwk7273/zmk-config-meteorite40/issues/17)) ([aa621cb](https://github.com/iwk7273/zmk-config-meteorite40/commit/aa621cb6aeffb4899e902939da530f844515c0d8))

### 修正

* ロータリーエンコーダーの時計回り・反時計回り設定が、電源再投入後に失われることがある問題を修正しました。

## [4.3.1](https://github.com/iwk7273/zmk-config-meteorite40/compare/v4.3.0...v4.3.1) (2026-07-03)


### 修正

* Meteorite Studio へ Bluetooth 経由で接続するための操作を、キー割り当てやコンボから選べるよう修正しました。 ([9659531](https://github.com/iwk7273/zmk-config-meteorite40/commit/96595318fbd86ba13b9f2bb970e9d9a5fd5f5bcf))

## 4.3.0 (2026-07-03)


### Features

* add Studio BLE discovery combo (Q+A+Z) and behavior include ([e064349](https://github.com/iwk7273/zmk-config-meteorite40/commit/e0643490f9a2cf4dd6695e783e29122e2aa8765a))
* **config:** add mixed encoder behaviors ([e2c86c3](https://github.com/iwk7273/zmk-config-meteorite40/commit/e2c86c3148237268aabcb3deaa3cf0cc2a2c3bf0))
* **config:** enable combo settings ([56dc629](https://github.com/iwk7273/zmk-config-meteorite40/commit/56dc6291d3ed3e45897c849abda00af466ac36c5))
* **config:** point meteorite firmware to rpc branches ([f8ad2c0](https://github.com/iwk7273/zmk-config-meteorite40/commit/f8ad2c0acf297ac798852221598292034f6cb0e0))
* **encoder:** expose encoder bindings as keymap slots ([baf3eff](https://github.com/iwk7273/zmk-config-meteorite40/commit/baf3eff3b0e4a9705ee2742843a509af25632916))
* **release:** report build version over RPC; automate releases ([b1b6bd0](https://github.com/iwk7273/zmk-config-meteorite40/commit/b1b6bd06bd9920f00443cb43cf2264c7855480cd))
* スクロール用 motion_scaler を追加 ([a3ca211](https://github.com/iwk7273/zmk-config-meteorite40/commit/a3ca211aada40f376806395f41a49feb590849f7))


### Bug Fixes

* **ball:** browser zoom via Ctrl/Cmd +=/- (consumer AC_ZOOM didn't work) ([1693884](https://github.com/iwk7273/zmk-config-meteorite40/commit/1693884082b63723a7090fd97b7c8903a2631a61))
* **ball:** default sensitivity macro to renumbered NORMAL (1-&gt;2) ([d5ce709](https://github.com/iwk7273/zmk-config-meteorite40/commit/d5ce7098b9c2d762e10668671b3e0180af6bea9e))
* **ball:** fill Mac no-op bindings for DESKTOP/WINDOW profiles ([b84bea4](https://github.com/iwk7273/zmk-config-meteorite40/commit/b84bea4b2d1805ece209428bd2e5483c0c174450))
* **ball:** restore DESKTOP DOWN to show-desktop toggle (LG(D)/F11) ([41edbc8](https://github.com/iwk7273/zmk-config-meteorite40/commit/41edbc89ce94673dcfe83764b84263fbbe66fbf5))
* **config:** add mixed low encoder behaviors ([22830ab](https://github.com/iwk7273/zmk-config-meteorite40/commit/22830ab70ffd056be2322d63a97b35b86d6ba090))
* **config:** enlarge Studio RPC buffers for combos ([973fcbb](https://github.com/iwk7273/zmk-config-meteorite40/commit/973fcbb31ba77ad2bef014a313b501c9935388b7))
* **config:** simplify encoder defaults ([dd1cfc9](https://github.com/iwk7273/zmk-config-meteorite40/commit/dd1cfc9529691b420721f77346bfca8b98d88a1a))
* **dt:** move ball_profile_defaults/custom_config_defaults out of #if CONFIG_ ([94d8d01](https://github.com/iwk7273/zmk-config-meteorite40/commit/94d8d018f8a6094e5a87bc8e728e85d804669540))
* increase Studio RPC TX buffer size for BLE transport ([6847cb4](https://github.com/iwk7273/zmk-config-meteorite40/commit/6847cb419f892cc97c3e1377f96f531ac3853fa8))
* increase Studio RPC TX buffer to 4096 for full layout response ([f646260](https://github.com/iwk7273/zmk-config-meteorite40/commit/f646260d08c7d468de5fcdcd28d52e366922764d))
* **studio:** set RPC TX buf to 512 alongside BLE streaming flush ([99a7907](https://github.com/iwk7273/zmk-config-meteorite40/commit/99a7907f540c545e6ad53516064149088e1433b5))


### Performance Improvements

* enable BLE DLE and larger MTU for Studio throughput ([c4df151](https://github.com/iwk7273/zmk-config-meteorite40/commit/c4df151a40080cc06483ebb771c4c98c908b9d39))


### Reverts

* **debug:** restore BLE profile test settings ([99ae7bf](https://github.com/iwk7273/zmk-config-meteorite40/commit/99ae7bfd81b78de04d977d702c1234e4f2dc829c))
