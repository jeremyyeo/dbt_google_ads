# dbt_google_ads v0.6.0
## 🚨 Breaking Changes 🚨
- The `account` source table has been renamed to be `account_history`. This has been reflected in the source model references within this release. ([#24](https://github.com/fivetran/dbt_google_ads_source/pull/24))
- The `ad_final_url_history` model has been removed from the connector. The url fields are now references within the `final_urls` field within the `ad_history` table. These changes are reflected in the `google_ads__url_adapter` model. ([#24](https://github.com/fivetran/dbt_google_ads_source/pull/24))
# dbt_google_ads v0.5.0
🎉 dbt v1.0.0 Compatibility 🎉
## 🚨 Breaking Changes 🚨
- Adjusts the `require-dbt-version` to now be within the range [">=1.0.0", "<2.0.0"]. Additionally, the package has been updated for dbt v1.0.0 compatibility. If you are using a dbt version <1.0.0, you will need to upgrade in order to leverage the latest version of the package.
  - For help upgrading your package, I recommend reviewing this GitHub repo's Release Notes on what changes have been implemented since your last upgrade.
  - For help upgrading your dbt project to dbt v1.0.0, I recommend reviewing dbt-labs [upgrading to 1.0.0 docs](https://docs.getdbt.com/docs/guides/migration-guide/upgrading-to-1-0-0) for more details on what changes must be made.
- Upgrades the package dependency to refer to the latest `dbt_google_ads_source`. Additionally, the latest `dbt_google_ads_source` package has a dependency on the latest `dbt_fivetran_utils`. Further, the latest `dbt_fivetran_utils` package also has a dependency on `dbt_utils` [">=0.8.0", "<0.9.0"].
  - Please note, if you are installing a version of `dbt_utils` in your `packages.yml` that is not in the range above then you will encounter a package dependency error.

# dbt_google_ads v0.1.0 -> v0.4.0
Refer to the relevant release notes on the Github repository for specific details for the previous releases. Thank you!
