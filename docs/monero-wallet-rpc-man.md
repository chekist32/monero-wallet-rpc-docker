```shell
Monero 'Fluorine Fermi' (v0.18.3.1-release)

This is the command line monero wallet. It needs to connect to a monero
daemon to work correctly.

Usage:
  monero-wallet-rpc [--wallet-file=<file>|--generate-from-json=<file>|--wallet-dir=<directory>] [--rpc-bind-port=<port>]

General options:
  --help                                Produce help message
  --version                             Output version information

Wallet options:
  --daemon-address arg                  Use daemon instance at <host>:<port>
  --daemon-host arg                     Use daemon instance at host <arg> 
                                        instead of localhost
  --proxy arg                           [<ip>:]<port> socks proxy to use for 
                                        daemon connections
  --trusted-daemon                      Enable commands which rely on a trusted
                                        daemon
  --untrusted-daemon                    Disable commands which rely on a 
                                        trusted daemon
  --password arg                        Wallet password (escape/quote as 
                                        needed)
  --password-file arg                   Wallet password file
  --daemon-port arg (=0)                Use daemon instance at port <arg> 
                                        instead of 18081
  --daemon-login arg                    Specify username[:password] for daemon 
                                        RPC client
  --daemon-ssl arg (=autodetect)        Enable SSL on daemon RPC connections: 
                                        enabled|disabled|autodetect
  --daemon-ssl-private-key arg          Path to a PEM format private key
  --daemon-ssl-certificate arg          Path to a PEM format certificate
  --daemon-ssl-ca-certificates arg      Path to file containing concatenated 
                                        PEM format certificate(s) to replace 
                                        system CA(s).
  --daemon-ssl-allowed-fingerprints arg List of valid fingerprints of allowed 
                                        RPC servers
  --daemon-ssl-allow-any-cert           Allow any SSL certificate from the 
                                        daemon
  --daemon-ssl-allow-chained            Allow user (via --daemon-ssl-ca-certifi
                                        cates) chain certificates
  --testnet                             For testnet. Daemon must also be 
                                        launched with --testnet flag
  --stagenet                            For stagenet. Daemon must also be 
                                        launched with --stagenet flag
  --shared-ringdb-dir arg (=/home/sokol/.shared-ringdb, /home/sokol/.shared-ringdb/testnet if 'testnet', /home/sokol/.shared-ringdb/stagenet if 'stagenet')
                                        Set shared ring database path
  --kdf-rounds arg (=1)                 Number of rounds for the key derivation
                                        function
  --bitmessage-address arg (=http://localhost:8442/)
                                        Use PyBitmessage instance at URL <arg>
  --bitmessage-login arg (=username:password)
                                        Specify <arg> as username:password for 
                                        PyBitmessage API
  --hw-device arg                       HW device to use
  --hw-device-deriv-path arg            HW device wallet derivation path (e.g.,
                                        SLIP-10)
  --tx-notify arg                       Run a program for each new incoming 
                                        transaction, '%s' will be replaced by 
                                        the transaction hash
  --no-dns                              Do not use DNS
  --offline                             Do not connect to a daemon, nor use DNS
  --extra-entropy arg                   File containing extra entropy to 
                                        initialize the PRNG (any data, aim for 
                                        256 bits of entropy to be useful, which
                                        typically means more than 256 bits of 
                                        data)
  --allow-mismatched-daemon-version     Allow communicating with a daemon that 
                                        uses a different version
  --rpc-bind-port arg                   Sets bind port for server
  --disable-rpc-login                   Disable HTTP authentication for RPC 
                                        connections served by this process
  --restricted-rpc                      Restricts to view-only commands
  --rpc-bind-ip arg (=127.0.0.1)        Specify IP to bind RPC server
  --rpc-bind-ipv6-address arg (=::1)    Specify IPv6 address to bind RPC server
  --rpc-restricted-bind-ip arg (=127.0.0.1)
                                        Specify IP to bind restricted RPC 
                                        server
  --rpc-restricted-bind-ipv6-address arg (=::1)
                                        Specify IPv6 address to bind restricted
                                        RPC server
  --rpc-use-ipv6                        Allow IPv6 for RPC
  --rpc-ignore-ipv4                     Ignore unsuccessful IPv4 bind for RPC
  --rpc-login arg                       Specify username[:password] required 
                                        for RPC server
  --confirm-external-bind               Confirm rpc-bind-ip value is NOT a 
                                        loopback (local) IP
  --rpc-access-control-origins arg      Specify a comma separated list of 
                                        origins to allow cross origin resource 
                                        sharing
  --rpc-ssl arg (=autodetect)           Enable SSL on RPC connections: 
                                        enabled|disabled|autodetect
  --rpc-ssl-private-key arg             Path to a PEM format private key
  --rpc-ssl-certificate arg             Path to a PEM format certificate
  --rpc-ssl-ca-certificates arg         Path to file containing concatenated 
                                        PEM format certificate(s) to replace 
                                        system CA(s).
  --rpc-ssl-allowed-fingerprints arg    List of certificate fingerprints to 
                                        allow
  --rpc-ssl-allow-chained               Allow user (via --rpc-ssl-certificates)
                                        chain certificates
  --disable-rpc-ban                     Do not ban hosts on RPC errors
  --wallet-file arg                     Use wallet <arg>
  --generate-from-json arg              Generate wallet from JSON format file
  --wallet-dir arg                      Directory for newly created wallets
  --prompt-for-password                 Prompts for password when not provided
  --rpc-client-secret-key arg           Set RPC client secret key for RPC 
                                        payments
  --no-initial-sync                     Skips the initial sync before listening
                                        for connections
  --detach                              Run as daemon
  --pidfile arg                         File path to write the daemon's PID to 
                                        (optional, requires --detach)
  --non-interactive                     Run non-interactive
  --log-file arg                        Specify log file
  --log-level arg                       0-4 or categories
  --max-log-file-size arg (=104850000)  Specify maximum log file size [B]
  --max-log-files arg (=50)             Specify maximum number of rotated log 
                                        files to be saved (no limit by setting 
                                        to 0)
  --max-concurrency arg (=0)            Max number of threads to use for a 
                                        parallel job
  --config-file arg                     Config file
```