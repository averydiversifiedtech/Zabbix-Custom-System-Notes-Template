# Zabbix-Custom-System-Notes-Template
Simple template for the recording of custom notes for hosts sent by Zabbix Sender.  Will alert on changed text.


Template with a single item and trigger for setting custom notes on each host.  Can use zabbix_sender to manually send info such as "check the scanner" - trigger alerts on change in the value and can be manually closed.

Can be triggered with the following from any system with zabbix sender and permissions to access the server:

zabbix_sender -c /etc/zabbix/zabbix_agentd.conf -s hostname -k custom.notes -o "This is a new note"

Nice and easy and an alert is triggered on a new value for that host.
