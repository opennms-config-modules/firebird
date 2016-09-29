# Firebird SQL Monitoring

OpenNMS configuration module to support Firebird SQL databases monitoring.
The configuration adds capabilities database connection test and performance data collection for the following metrics:

- Client Connection Count (active/inactive)
- Transaction Count (active/inactive)
- Statement Count (active/inactive)

## Requirements

- Firebird SQL Server 2.5 http://www.firebirdsql.org/en/server-packages/
- Jaybird Driver http://www.firebirdsql.org/en/jdbc-driver/
- OpenNMS Meridian 2015+ or OpenNMS Horizon 14+

## Install Jaybird

* Download and extract the Jaybird files and copy **jaybird*.jar*** into $OPENNMS_HOME/lib

## Config Collectd

* copy the collectd example into your config and update the **UPPERCASE** variables to your need
* **!!!** Put your Firebird node into surveillance category **FirebirdSQL**

## Config JDBC

* copy the jdbc-collection example into your config and update the **UPPERCASE** variables to your need

## Config Graphs

* copy the graph defintion file into ***$OPENNMS_HOME/etc/snmp-graph.properties.d/***

## Config Poller

If you need to check the database connection as a OpenNMS service, follow these steps:

* add a service to your Firebird node (eg. named ***DATABASE-NAME***)
* copy the pollerd example into your config and update the **UPPERCASE** variables to your need

## Final step

* restart OpenNMS to load the new configuration

# License & Authors

- Author:: Marcel Fuhrmann <fuhrmann@n3rd.org>

Licensed under the GNU Affero General Public License 3+. You may obtain a copy of the License at http://www.gnu.org/licenses/agpl-3.0.html.
