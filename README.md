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

## Download the configuration package

.Download the configuration files
[source, bash]
----
mkdir /tmp
cd /tmp
curl -L https://github.com/opennms-config-modules/firebird/archive/master.tar.gz | tar xz
cd firebird
----

## Install Jaybird


## Config Collectd

## Config JDBC

## Config Poller

## Config Graphs

# License & Authors

- Author:: Marcel Fuhrmann <fuhrmann@n3rd.org>

Licensed under the GNU Affero General Public License 3+. You may obtain a copy of the License at http://www.gnu.org/licenses/agpl-3.0.html.
