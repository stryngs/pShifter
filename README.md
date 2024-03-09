# pShifter
Anonymize a given pcap by changing identifiable markers within the pcap.

The first iteration of this code will focus on frames gathered in monitor mode
and operate at layer 2 for pcap anonymization.

This code uses a random mac generator and tracks what changed.  The original
pcap is left untouched and a new one using the same name with a prefix of
shifted_ is created.  theShift.log is a list that shows all mac addresses found
and their subsequent change.

Future revisions will work at other layers such as TCP and UDP for further
anonymization options as well as offering hardcoded mac options on the shifting.
