# hidden
xor encoded files for pentest purposes

decode with:
((gc .\mimicats.ps1 -ReadCount 0) -split '' | %{[char]([char]$_ -bxor 5)}) -join ''

mimicats.ps1  0x05
