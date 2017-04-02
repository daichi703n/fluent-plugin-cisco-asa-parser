# Cisco ASA Fluent Parser

This project is forked from [rogeriobastos/fluent-plugin-cisco-asa-parser](https://github.com/rogeriobastos/fluent-plugin-cisco-asa-parser)

Because the project is seemed to be finished to maintenance, I'm trying to continue update.

## How to use

1. Clone this repository or Download `parser_cisco_asa.rb`.
2. Put `parser_cisco_asa.rb` to `/etc/td-agent/plugin/`.
3. In configuration file, set type to **cisco_asa**.

### Sample Configuration
Sample Fluentd (td-agent) configuration. This snip contains source only. Please create the match direactive.

```
<source>
  @type tail
  path /var/log/ASA5505.log
  pos_file /var/log/ASA5505.log.pos
  tag net.asa5505.<hostname>
  format cisco_asa
</source>
```

## Contact
Please create the issue.

