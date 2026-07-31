# OpenLane Commands

## Linux Basics
```bash
pwd
ls
ls -ltr
cd
mkdir
rm
cp
mv
cat
grep
find
clear
history
```

## GitHub Codespaces
```bash
make test
```

## OpenLane
```bash
./flow.tcl -interactive
prep -design <design_name>
run_synthesis
run_floorplan
run_placement
run_cts
run_routing
```

## Magic
```bash
magic
drc check
drc why
extract all
ext2spice
```

## ngspice
```bash
ngspice file.spice
plot v(out)
```

## STA
```tcl
report_checks
report_tns
report_wns
```

## Useful Tips
- Use `Tab` for auto-completion.
- Linux commands are case-sensitive.
- Use `Ctrl + C` to stop a running command.
- Use `history` to view previous commands.
