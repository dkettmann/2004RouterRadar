# 2004RouterRadar
Historical Archive of Perl scripts written in 2004 - RouterRadar aka ChgTrkr

I wrote these scripts in aprox 2003-2004 for a previous employer.

From what I remember, this program was a BEAST.  My partner in crime Fabricio and I saw a shot and we took it.  We supported
a network of aprox 2000 branch sites and we really wanted to know if any of the configs had changed on them and what had changed.
We wanted it to run overnight and in the morning it would generate an HTML report and say "Branch XXXX had a different config than the
previous night when we captured it, here is the diff output."  Management was *very* happy with this one if I recall correctly.
It did a lot with what we knew and had at the time. 

Also included is brlistgen, which would bug the hell out of the DNS server asking if any possible branch IP address had a name, and
if so would put that branch name/IP in to a list.  That generated list would be the one that RADAR used for its nightly job, making DNS a
type of single-source-of-truth for branch listing.

I should revisit this one and write more, a lot of thought and work went in to it. It was fun to work with the Expect module in Perl.
Also I did blow away one password from this script -- I realized my current medium security password was once-upon-a-time the one
I used for this job's enable pass.

Also I added the "translate" script because I think it was an intermediate step in generating the report after it ran maybe?
....and the crontab that kicked off the script for each ICORE (aprox 700 sites each).
