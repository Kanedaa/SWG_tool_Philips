This is a straightforward Python 3 script that has been converted into an executable (.exe) application for Windows10/11 hosts.

Administrative privileges are necessary for its operation. As this code is not digitally signed or endorsed by Microsoft, 
adjustments to the security settings of the test host may be required.



Test #1:

The first test involves performing a ping check on a list of IP addresses available at: https://geofeed.network.strln.net. 
The process involves examining all subnets associated with each SWG Data Center (DC) to identify which IPs respond to the ping request.

Test #2:

The second test resolves the domain swg-url-proxy-https.sigproxy.qq.opendns.com using OpenDNS resolvers, 
and the initial result is printed immediately upon launching the tool. The second result is produced after initiating the test and involves resolving the same domain against the DNS configuration set locally on the host.

Customers may reconfigure the host's DNS server and repeat the test. Depending on the DNS server's location, 
it should theoretically indicate the nearest SWG to that server.

Test #3

The third test leverages information from the swg_dc.json list, which is hosted on GitHub. This test executes a series of ping tests (both ICMP and TCP) and subsequently verifies whether the selected IP address is listening on port 80.

Please note that the application requires access to the following directories:

    C:\ProgramData\Cisco\Cisco Secure Client\Umbrella\data\
    C:\ProgramData\Cisco\Cisco Secure Client\Umbrella\SWG\

Additionally, it is necessary to have permission to manage services, as this is essential for starting and stopping the csc_vpnagent process.

It is important to mention that this test is not flawless; other IPs dedicated to SWG range may also be listening on port 80. Moreover, due to CAPTCHA restrictions on the page at https://cachecheck.opendns.com/, automation of this test is currently not feasible.

In the future, if time permits, I may attempt to enhance the reliability of this third test.



--------------------------------------------------------------------------------------------

If you would like to share feedback, please feel free to reach out via email or LinkedIn.
kporzezr@cisco.com
https://www.linkedin.com/in/konrad-porzezynski/
