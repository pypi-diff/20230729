# Comparing `tmp/undervolt-0.3.0.tar.gz` & `tmp/undervolt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/undervolt-0.3.0.tar", last modified: Sat May  9 12:29:20 2020, max compression
+gzip compressed data, was "undervolt-0.4.0.tar", last modified: Sat Jul 29 14:00:25 2023, max compression
```

## Comparing `undervolt-0.3.0.tar` & `undervolt-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 grw       (1000) users      (100)        0 2020-05-09 12:29:20.000000 undervolt-0.3.0/
--rw-r--r--   0 grw       (1000) users      (100)    11683 2020-05-09 12:29:20.000000 undervolt-0.3.0/PKG-INFO
--rw-r--r--   0 grw       (1000) users      (100)     9046 2020-05-09 12:23:47.000000 undervolt-0.3.0/README.rst
--rw-r--r--   0 grw       (1000) users      (100)       38 2020-05-09 12:29:20.000000 undervolt-0.3.0/setup.cfg
--rw-r--r--   0 grw       (1000) users      (100)      999 2020-05-09 12:15:51.000000 undervolt-0.3.0/setup.py
-drwxr-xr-x   0 grw       (1000) users      (100)        0 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/
--rw-r--r--   0 grw       (1000) users      (100)    11683 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/PKG-INFO
--rw-r--r--   0 grw       (1000) users      (100)      200 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/SOURCES.txt
--rw-r--r--   0 grw       (1000) users      (100)        1 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/dependency_links.txt
--rw-r--r--   0 grw       (1000) users      (100)       46 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/entry_points.txt
--rw-r--r--   0 grw       (1000) users      (100)       10 2020-05-09 12:29:20.000000 undervolt-0.3.0/undervolt.egg-info/top_level.txt
--rwxr-xr-x   0 grw       (1000) users      (100)    16137 2020-05-09 12:23:47.000000 undervolt-0.3.0/undervolt.py
+drwxr-xr-x   0 grw       (1000)     1000        0 2023-07-29 14:00:25.337860 undervolt-0.4.0/
+-rw-r--r--   0 grw       (1000)     1000      596 2023-07-29 13:54:36.000000 undervolt-0.4.0/LICENSE.txt
+-rw-r--r--   0 grw       (1000)     1000    11307 2023-07-29 14:00:25.337860 undervolt-0.4.0/PKG-INFO
+-rw-r--r--   0 grw       (1000)     1000    10819 2023-07-29 13:54:36.000000 undervolt-0.4.0/README.rst
+-rw-r--r--   0 grw       (1000)     1000       38 2023-07-29 14:00:25.337860 undervolt-0.4.0/setup.cfg
+-rw-r--r--   0 grw       (1000)     1000      999 2023-07-29 13:54:36.000000 undervolt-0.4.0/setup.py
+drwxr-xr-x   0 grw       (1000)     1000        0 2023-07-29 14:00:25.336860 undervolt-0.4.0/undervolt.egg-info/
+-rwxrwxrwx   0 grw       (1000)     1000    11307 2023-07-29 14:00:25.000000 undervolt-0.4.0/undervolt.egg-info/PKG-INFO
+-rwxrwxrwx   0 grw       (1000)     1000      212 2023-07-29 14:00:25.000000 undervolt-0.4.0/undervolt.egg-info/SOURCES.txt
+-rwxrwxrwx   0 grw       (1000)     1000        1 2023-07-29 14:00:25.000000 undervolt-0.4.0/undervolt.egg-info/dependency_links.txt
+-rwxrwxrwx   0 grw       (1000)     1000       45 2023-07-29 14:00:25.000000 undervolt-0.4.0/undervolt.egg-info/entry_points.txt
+-rwxrwxrwx   0 grw       (1000)     1000       10 2023-07-29 14:00:25.000000 undervolt-0.4.0/undervolt.egg-info/top_level.txt
+-rwxr-xr-x   0 grw       (1000)     1000    17141 2023-07-29 13:59:33.000000 undervolt-0.4.0/undervolt.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `undervolt-0.3.0/README.rst` & `undervolt-0.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -6,61 +6,71 @@
 
 .. |travis| image:: https://travis-ci.org/georgewhewell/undervolt.svg
     :target: https://travis-ci.org/georgewhewell/undervolt
     :alt: Build Status
 
 *undervolt* is a program for undervolting Intel CPUs under Linux. It works in
 a similar manner to the Windows program *ThrottleStop* (i.e, `MSR 0x150`). You
-can apply a fixed voltage offset to one of 5 voltage planes, and override your
-systems temperature target (CPU will throttle when this temperature is reached).
+can apply a fixed voltage offset to one of 5 voltage planes, override your
+systems temperature target (CPU will throttle when this temperature is reached),
+and adjust the system's short and long power budgets (clocks and thus voltages
+will be altered in order to keep total power usage in these periods under the
+configured limits).
 
 For more information, read
 `here <https://github.com/mihic/linux-intel-undervolt>`_.
 
 Installing
 ----------
 
 From PyPi::
 
     $ pip install undervolt
 
 From source::
 
-    $ git clone https://github.com/georgewhewell/undervolt.git
+    $ pip install git+https://github.com/georgewhewell/undervolt.git    
+    
+Note for custom kernel users: the module 'msr' ("CONFIG_X86_MSR") must be enabled in the kernel options (Processor type & features -> Model-specific register support)
 
 Examples
 --------
 
 Read current offsets::
 
     $ undervolt --read
     temperature target: -25 (75C)
     core: -110.35 mV
     gpu: -49.8 mV
     cache: -110.35 mV
     uncore: -59.57 mV
     analogio: -59.57 mV
     powerlimit: 35.0W (short: 1.0s - enabled) / 35.0W (long: 1.0s - enabled)
+    turbo: enabled
 
-Apply -100mV offset to CPU Core and Cache::
+Apply -100mV offset to CPU Core and Cache:
 
     $ undervolt --core -100 --cache -100
 
-Apply -75mV offset to GPU, -100mV to all other planes::
+Apply -75mV offset to GPU, -100mV to all other planes:
 
     $ undervolt --gpu -75 --core -100 --cache -100 --uncore -100 --analogio -100
 
-Set temperature target to 97C::
+Set temperature target to 97C:
 
     $ undervolt --temp 97
 
 Set powerlimit 1 to 35W, 10s:
 
     $ undervolt -p1 35 10
 
+Set Intel Turbo disabled:
+
+    $ undervolt --turbo 1
+
 Generated the command to run to recreate your Throttlestop settings::
 
     $ undervolt --throttlestop ThrottleStop.ini --tsindex 3
     undervolt --core -100.5859375
     $ undervolt --throttlestop ThrottleStop.ini
     undervolt --core -125.0 --gpu -125.0 --cache -125.0
 
@@ -79,14 +89,15 @@
 
     optional arguments:
       -h, --help            show this help message and exit
       --version             show program's version number and exit
       -v, --verbose         print debug info
       -f, --force           allow setting positive offsets
       -r, --read            read existing values
+      --turbo               Changes the Intel Turbo feature status (1 is disabled and 0 is enabled)
       -t TEMP, --temp TEMP  set temperature target on AC (and battery power if
                             --temp-bat is not used)
       --temp-bat TEMP_BAT   set temperature target on battery power
       --throttlestop THROTTLESTOP
                             extract values from ThrottleStop
       --tsindex TSINDEX     ThrottleStop profile index
       -p1 POWER_LIMIT TIME_WINDOW, --power-limit-long POWER_LIMIT TIME_WINDOW
@@ -185,57 +196,73 @@
   $ sudo ln -s /etc/sv/undervolt /var/services/
 
 Hardware support
 ----------------
 
 Undervolting should work on any CPU later than Haswell.
 
-============================ ========= ==========
-      System                    CPU     Working? 
-============================ ========= ==========
-Acer Aspire 7 (A715-71G)     i5-7300HQ Yes
-Acer Aspire E 15 (E5-575G)   i5-7200U  Yes
-Acer Nitro 5                 i5-7300HQ Yes
-Acer Nitro 5  (An515-52)     i5-8300H  Yes
-Asus FX504GE                 i7-8750H  Yes
-Asus GL703GE                 i7-8750H  Yes
-Dell G5                      i7-8750H  Yes
-Dell Latitude 5400           i7-8665U  Yes
-Dell Latitude 5480           i5-6300U  Yes
-Dell Latitude 7390           i7-8650U  Yes
-Dell Precision 5530          i9-8950HK Yes
-Dell Precision M3800         i7-4712HQ Yes
-Dell Precision 7530          i9-8950HK Yes
-Dell Precision 7730          E-2176M   Yes
-Dell Precision 7740          E-2286M   Yes
-Dell XPS 13 9343             i5-5200U  Yes
-Dell XPS 13 9360             i7-7560U  Yes
-Dell XPS 15 9530             i7-4712HQ Yes
-Dell XPS 15 9550             i7-6700HQ Yes
-Dell XPS 15 9560             i7-7700HQ Yes
-Dell XPS 15 9570             i9-8950HK Yes
-Dell XPS 15 9575             i7-8705G  Yes
-Dell XPS 15 7590             i9-9980HK Yes
-HP Spectre X360              i7-8809G  Yes
-HP Zbook Studio G5           i7-8750H  Yes
-Lenovo Thinkpad T440p        i5-4300M  Yes
-Lenovo Thinkpad T470p        i7-7700HQ Yes
-Lenovo Thinkpad x250         i7-5600U  Yes
-Lenovo Thinkpad X1 Carbon    i7-6600U  Yes
-Lenovo Thinkpad X1 Extreme   i7-8750H  Yes
-Lenovo X1 Gen 5              i7-7500U  Yes
-Lenovo X1 Yoga Gen 2         i7-7600U  Yes
-Lenovo Yoga 920              i7-8550U  Yes
-MacBook Air Mid 2013         i5-4250U  Yes
-MacBook Air Late 2015        i5-5250U  Yes
-MSI GP73 Leopard 8RF         i7-8750H  Yes
-Lenovo Thinkpad T430         i7-3610QM No
-Toshiba Chromebook 2         N2840     No
-
-============================ ========= ==========
+================================== ========= ==========
+      System                          CPU     Working?
+================================== ========= ==========
+Acer Aspire 7 (A715-71G)           i5-7300HQ Yes
+Acer Aspire E 15 (E5-575G)         i5-7200U  Yes
+Acer Nitro 5                       i5-7300HQ Yes
+Acer Nitro 5  (An515-52)           i5-8300H  Yes
+Acer Predator (PH315-51)           i7-8750H  Yes
+Acer Swift 7 (SF714)               i5-8200Y  Yes 
+Asus FX504GE                       i7-8750H  Yes
+Asus GL703GE                       i7-8750H  Yes
+Dell G5                            i7-8750H  Yes
+Dell G5 5590                       i7-9750H  Yes
+Dell Inspiron 5577                 i7-7700HQ  Yes
+Dell Inspiron 7560                 i7-7500U  Yes
+Dell Latitude 3301                 i5-8265U  Yes
+Dell Latitude 5400                 i7-8665U  Yes
+Dell Latitude 5480                 i5-6300U  Yes
+Dell Latitude 7390                 i7-8650U  Yes
+Dell Precision 5530                i9-8950HK Yes
+Dell Precision 7530                i9-8950HK Yes
+Dell Precision 7730                E-2176M   Yes
+Dell Precision 7740                E-2286M   Yes
+Dell Precision M3800               i7-4712HQ Yes
+Dell XPS 13 9343                   i5-5200U  Yes
+Dell XPS 13 9350                   i7-6560U  Yes
+Dell XPS 13 9360                   i7-7560U  Yes
+Dell XPS 15 7590                   i7-9750H  Yes
+Dell XPS 15 7590                   i9-9980HK Yes
+Dell XPS 15 9530                   i7-4712HQ Yes
+Dell XPS 15 9550                   i7-6700HQ Yes
+Dell XPS 15 9560                   i7-7700HQ Yes
+Dell XPS 15 9570                   i9-8950HK Yes
+Dell XPS 15 9575                   i7-8705G  Yes
+HP Omen 17-an061ur                 i7-7700HQ Yes
+HP Spectre X360                    i7-8809G  Yes
+HP Zbook Studio G5                 i7-8750H  Yes
+Intel NUC7i3BNK                    i3-7100U  Yes
+Lenovo AIO Y910 27ISH              i7-6700   Yes
+Lenovo IdeaCentre Q190             1017U     No
+Lenovo Thinkpad T430               i7-3610QM No
+Lenovo Thinkpad T440p              i5-4300M  Yes
+Lenovo Thinkpad T470p              i7-7700HQ Yes
+Lenovo Thinkpad T470p              i7-7820HQ Yes
+Lenovo Thinkpad T480s              i5-8250U  Yes
+Lenovo Thinkpad T490               i5-8265U  Yes
+Lenovo Thinkpad X1 Carbon          i7-6600U  Yes
+Lenovo Thinkpad X1 Extreme         i7-8750H  Yes
+Lenovo Thinkpad X1 Extreme Gen 2   i7-9750H  Yes
+Lenovo Thinkpad x250               i7-5600U  Yes
+Lenovo X1 Gen 5                    i7-7500U  Yes
+Lenovo X1 Yoga Gen 2               i7-7600U  Yes
+Lenovo Yoga 920                    i7-8550U  Yes
+MSI GE60 2QD Apache                i7-4720HQ Yes
+MSI GP73 Leopard 8RF               i7-8750H  Yes
+MacBook Air Late 2015              i5-5250U  Yes
+MacBook Air Mid 2013               i5-4250U  Yes
+Toshiba Chromebook 2               N2840     No
+================================== ========= ==========
 
 Troubleshooting
 ---------------
 
 - **Core or Cache offsets have no effect.**
   It is not possible to set different offsets for CPU Core and Cache. The CPU
   will take the smaller of the two offsets, and apply that to both CPU and
@@ -245,14 +272,15 @@
 - ``OSError: [Errno 1] Operation not permitted``
   First try running with ``sudo``. If the error persists, your system is
   probably booted in Secure Boot mode. In this case, the Linux kernel will
   prevent userspace programs (even as root) from writing to the CPU's
   model-specific registers. Disable UEFI Secure Boot in your system's BIOS
   and the error should go away.
 
+- Undervolt has no effect - Your device BIOS might be blocking it. Check the wiki (https://github.com/georgewhewell/undervolt/wiki) to find notes for your hardware
 
 GUI
 ----------------
 There is also a small gui written in Java avaiable here: https://github.com/zmalrobot/JavaLinuxUndervolt
 
 It will allow you to set each value core, gpu, cache, uncore, analogio (temperature target isn't implemented yet),save a profile, load a profile and reset the value.
```

### Comparing `undervolt-0.3.0/setup.py` & `undervolt-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `undervolt-0.3.0/undervolt.py` & `undervolt-0.4.0/undervolt.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 try: # Python >=3.3
     from math import log2
 except ImportError:
     from math import log
     def log2(x):
         return log(x, 2)
-__version__ = '0.3.0'
+
+__version__ = '0.4.0'
 
 AC_STATE_NODE = os.environ.get(
     'AC_STATE_NODE', (glob('/sys/class/power_supply/AC*/online') + [None])[0])
 PLANES = {
     'core': 0,
     'gpu': 1,
     'cache': 2,
@@ -65,14 +66,16 @@
 
 def write_msr(val, addr):
     """
     Use /dev/cpu/*/msr interface provided by msr module to read/write
     values from register addr.
     Writes to all msr node on all CPUs available.
     """
+    assert_root()
+    
     for i in valid_cpus():
         c = '/dev/cpu/%d/msr' % i
         if not os.path.exists(c):
             raise OSError("msr module not loaded (run modprobe msr)")
         logging.info("Writing {val} to {msr}".format(val=hex(val), msr=c))
         f = os.open(c, os.O_WRONLY)
         os.lseek(f, addr, os.SEEK_SET)
@@ -80,14 +83,16 @@
         os.close(f)
 
 
 def read_msr(addr, cpu=0):
     """
     Read a value from single msr node on given CPU (defaults to first)
     """
+    assert_root()
+
     n = '/dev/cpu/%d/msr' % (cpu,)
     f = os.open(n, os.O_RDONLY)
     os.lseek(f, addr, os.SEEK_SET)
     val, = unpack('Q', os.read(f, 8))
     logging.info("Read {val} from {n}".format(val=hex(val), n=n))
     os.close(f)
     return val
@@ -344,23 +349,30 @@
     Returns True if AC is connected, else False
     """
     if AC_STATE_NODE:
         return open(AC_STATE_NODE).read() == '1\n'
     # Assume no battery if the /sys entry is missing.
     return True
 
+def assert_root():
+    """
+    Checks whether the user has root privileges, exit otherwise
+    """
+    if os.geteuid() != 0:
+        exit("You need to have root privileges to run this script with these options.\nRerun with 'sudo'.")
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', action='version', version='%(prog)s {version}'.format(version=__version__))
     parser.add_argument('-v', '--verbose', action='store_true',
                         help="print debug info")
     parser.add_argument('-f', '--force', action='store_true',
                         help="allow setting positive offsets")
     parser.add_argument('-r', '--read', action="store_true", help="read existing values")
+    parser.add_argument('--turbo', type=int, help="Changes the Intel Turbo feature status (1 is disabled and 0 is enabled)")
     parser.add_argument('-t', '--temp', type=int, help="set temperature target on AC (and battery power if --temp-bat is not used)")
     parser.add_argument('--temp-bat', type=int, help="set temperature target on battery power")
     parser.add_argument('--throttlestop', type=str,
                         help="extract values from ThrottleStop")
     parser.add_argument('--tsindex', type=int,
                         default=0, help="ThrottleStop profile index")
     parser.add_argument('-p1', '--power-limit-long', nargs=2, help="P1 Power Limit (W) and Time Window (s)", metavar=('POWER_LIMIT', 'TIME_WINDOW'))
@@ -382,15 +394,15 @@
     
     msr = ADDRESSES
 
     if not glob('/dev/cpu/*/msr'):
         subprocess.check_call(['modprobe', 'msr'])
 
     if (args.core or args.cache) and args.core != args.cache:
-        logging.warn(
+        logging.warning(
             "You have supplied different offsets for Core and Cache. "
             "The smaller of the two (or none if you only supplied one) will be applied to both planes."
         )
 
     # for each arg, try to set voltage
     for plane in PLANES:
         offset = getattr(args, plane)
@@ -451,10 +463,24 @@
             power_limit.short_term_time,
             'enabled' if power_limit.short_term_enabled else 'disabled',
             power_limit.long_term_power,
             power_limit.long_term_time,
             'enabled' if power_limit.long_term_enabled else 'disabled',
             ' [locked]' if power_limit.locked else ''
         ))
+        with open("/sys/devices/system/cpu/intel_pstate/no_turbo","r") as file:
+            turboDisable = int(file.readline())
+            print('turbo: {}'.format("disable" if turboDisable == 1 else "enable"))
+    
+    turbo = getattr(args, 'turbo')
+    if turbo is not None:
+        intelTurboState = int(turbo)
+        if intelTurboState == 0:
+            print("New Intel Turbo State ENABLED")
+        else:
+            print("New Intel Turbo State DISABLED")
+        
+        with open("/sys/devices/system/cpu/intel_pstate/no_turbo","w+") as file:
+            file.write(str(intelTurboState))
 
 if __name__ == '__main__':
     main()
```

