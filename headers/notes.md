mistery_binery_ai_wallets$ x86_64-w64-mingw32-objdump -p ../ETH\ Seed\ \&\ Keys\ Converter\ @ai_wallets/ETH\ Seed\ \&\ Keys\ Converter.exe | grep -i -E "Entry|ImageBase|Magic|SizeOf"
Magic			020b	(PE32+)
SizeOfCode		000000000002a600
SizeOfInitializedData	0000000000027a00
SizeOfUninitializedData	0000000000000000
AddressOfEntryPoint	000000000000ce20
ImageBase		0000000140000000
SizeOfImage		0005b000
SizeOfHeaders		00000400
SizeOfStackReserve	00000000001e8480
SizeOfStackCommit	0000000000001000
SizeOfHeapReserve	0000000000100000
SizeOfHeapCommit	0000000000001000
Entry 0 0000000000000000 00000000 Export Directory [.edata (or where ever we found it)]
Entry 1 000000000003dd04 00000078 Import Directory [parts of .idata]
Entry 2 0000000000049000 00010e34 Resource Directory [.rsrc]
Entry 3 0000000000045000 0000228c Exception Directory [.pdata]
Entry 4 0000000000000000 00000000 Security Directory
Entry 5 000000000005a000 00000764 Base Relocation Directory [.reloc]
Entry 6 000000000003b1e0 0000001c Debug Directory
Entry 7 0000000000000000 00000000 Description Directory
Entry 8 0000000000000000 00000000 Special Directory
Entry 9 0000000000000000 00000000 Thread Storage Directory [.tls]
Entry a 000000000003b0a0 00000140 Load Configuration Directory
Entry b 0000000000000000 00000000 Bound Import Directory
Entry c 000000000002c000 000004b0 Import Address Table Directory
Entry d 0000000000000000 00000000 Delay Import Directory
Entry e 0000000000000000 00000000 CLR Runtime Header
Entry f 0000000000000000 00000000 Reserved
	3e820	 1289  RtlLookupFunctionEntry
010   Entry: ID: 0x000003, Value: 0x80000028
038     Entry: ID: 0x000001, Value: 0x80000070
080       Entry: ID: 00000000, Value: 0x0000b8
018   Entry: ID: 0x00000e, Value: 0x80000040
050     Entry: ID: 0x000001, Value: 0x80000088
098       Entry: ID: 00000000, Value: 0x0000c8
020   Entry: ID: 0x000018, Value: 0x80000058
068     Entry: ID: 0x000001, Value: 0x800000a0
0b0       Entry: ID: 00000000, Value: 0x0000d8
mistery_binery_ai_wallets$ 