::: note
::: title
Note
:::

For backups and restoration, Aiven utilises the popular Open Source
backup daemon `PGHoard <Terminology PGHoard>`{.interpreted-text
role="ref"}, which Aiven maintains. It makes real-time copies of
`WAL<Terminology PGWAL>`{.interpreted-text role="ref"} files to an
object store in compressed and encrypted format.
:::

You can also use the dedicated functions
`service logs <avn-service-logs>`{.interpreted-text role="doc"} and
`service metrics <avn-service-metrics>`{.interpreted-text role="doc"} to

Additionally, you have the option to
`export logs and metrics to an Aiven service or external provider</docs/platform/concepts/logs-metrics-alerts>`{.interpreted-text
role="doc"}, expanding your monitoring capabilities. For example:

-   You can send logs to
    `Aiven for Opensearch</docs/products/opensearch>`{.interpreted-text
    role="doc"}.
-   You can send metrics to
    `Aiven for m3</docs/products/m3db>`{.interpreted-text role="doc"},
    and visualise these metrics with
    `Aiven for Grafana</docs/products/grafana>`{.interpreted-text
    role="doc"}.

Or, you can use the `avn`
`command-line tool </docs/tools/cli>`{.interpreted-text role="doc"} with
the following command:

    avn service user-creds-download --username <username> <service-name>
