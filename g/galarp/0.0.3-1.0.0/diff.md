# Comparing `tmp/galarp-0.0.3.tar.gz` & `tmp/galarp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galarp-0.0.3.tar", last modified: Mon Apr  1 22:47:35 2024, max compression
+gzip compressed data, was "galarp-1.0.0.tar", last modified: Fri Mar 22 22:26:16 2024, max compression
```

## Comparing `galarp-0.0.3.tar` & `galarp-1.0.0.tar`

### file list

```diff
@@ -1,48 +1,21 @@
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.788655 galarp-0.0.3/
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1086 2024-03-26 19:05:50.000000 galarp-0.0.3/LICENSE
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1350 2024-04-01 22:47:35.788381 galarp-0.0.3/PKG-INFO
--rw-r--r--   0 hsouchereau   (503) staff       (20)      540 2024-03-28 19:36:22.000000 galarp-0.0.3/README.rst
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.782371 galarp-0.0.3/galarp/
--rw-r--r--   0 hsouchereau   (503) staff       (20)      413 2024-04-01 22:47:27.000000 galarp-0.0.3/galarp/__init__.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.784554 galarp-0.0.3/galarp/builtins/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       77 2024-03-29 15:17:44.000000 galarp-0.0.3/galarp/builtins/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1342 2024-03-28 20:47:49.000000 galarp-0.0.3/galarp/builtins/hosts.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      691 2024-03-28 18:25:11.000000 galarp-0.0.3/galarp/builtins/initconditions.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1118 2024-04-01 17:27:27.000000 galarp-0.0.3/galarp/builtins/satellites.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.785046 galarp-0.0.3/galarp/builtins/tests/
--rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-03-28 13:54:47.000000 galarp-0.0.3/galarp/builtins/tests/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1372 2024-04-01 15:20:26.000000 galarp-0.0.3/galarp/builtins/tests/test_builtins.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.785830 galarp-0.0.3/galarp/hosts/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       80 2024-03-29 15:07:15.000000 galarp-0.0.3/galarp/hosts/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      880 2024-03-29 16:44:51.000000 galarp-0.0.3/galarp/hosts/densities.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     3142 2024-04-01 15:21:10.000000 galarp-0.0.3/galarp/hosts/hostorbits.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      264 2024-04-01 15:16:44.000000 galarp-0.0.3/galarp/hosts/initconditions.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     9560 2024-04-01 22:04:44.000000 galarp-0.0.3/galarp/particle_grids.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.786278 galarp-0.0.3/galarp/postprocessing/
--rw-r--r--   0 hsouchereau   (503) staff       (20)       70 2024-04-01 22:01:07.000000 galarp-0.0.3/galarp/postprocessing/__init__.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.786878 galarp-0.0.3/galarp/postprocessing/plotting/
--rw-r--r--   0 hsouchereau   (503) staff       (20)      144 2024-04-01 22:03:44.000000 galarp-0.0.3/galarp/postprocessing/plotting/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     6382 2024-04-01 22:20:36.000000 galarp-0.0.3/galarp/postprocessing/plotting/general_plots.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1850 2024-04-01 22:01:41.000000 galarp-0.0.3/galarp/postprocessing/plotting/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     4734 2024-04-01 21:48:21.000000 galarp-0.0.3/galarp/postprocessing/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     6876 2024-04-01 22:00:59.000000 galarp-0.0.3/galarp/rampressure.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     8030 2024-03-26 19:05:50.000000 galarp-0.0.3/galarp/shadows.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.788040 galarp-0.0.3/galarp/tests/
--rw-r--r--   0 hsouchereau   (503) staff       (20)        0 2024-03-26 19:05:50.000000 galarp-0.0.3/galarp/tests/__init__.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      693 2024-04-01 16:19:47.000000 galarp-0.0.3/galarp/tests/helpers.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      462 2024-04-01 16:20:03.000000 galarp-0.0.3/galarp/tests/test_grids.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      495 2024-03-28 15:20:01.000000 galarp-0.0.3/galarp/tests/test_shadows.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1187 2024-04-01 22:36:08.000000 galarp-0.0.3/galarp/tests/test_utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      732 2024-03-28 21:18:39.000000 galarp-0.0.3/galarp/tests/test_winds.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)      659 2024-03-28 21:18:39.000000 galarp-0.0.3/galarp/tests.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     3435 2024-04-01 22:30:08.000000 galarp-0.0.3/galarp/utils.py
--rw-r--r--   0 hsouchereau   (503) staff       (20)     6495 2024-04-01 20:32:41.000000 galarp-0.0.3/galarp/winds.py
-drwxr-xr-x   0 hsouchereau   (503) staff       (20)        0 2024-04-01 22:47:35.783573 galarp-0.0.3/galarp.egg-info/
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1350 2024-04-01 22:47:35.000000 galarp-0.0.3/galarp.egg-info/PKG-INFO
--rw-r--r--   0 hsouchereau   (503) staff       (20)      977 2024-04-01 22:47:35.000000 galarp-0.0.3/galarp.egg-info/SOURCES.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)        1 2024-04-01 22:47:35.000000 galarp-0.0.3/galarp.egg-info/dependency_links.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)       30 2024-04-01 22:47:35.000000 galarp-0.0.3/galarp.egg-info/requires.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)        7 2024-04-01 22:47:35.000000 galarp-0.0.3/galarp.egg-info/top_level.txt
--rw-r--r--   0 hsouchereau   (503) staff       (20)      139 2024-03-28 20:47:19.000000 galarp-0.0.3/pyproject.toml
--rw-r--r--   0 hsouchereau   (503) staff       (20)       38 2024-04-01 22:47:35.788710 galarp-0.0.3/setup.cfg
--rw-r--r--   0 hsouchereau   (503) staff       (20)     1207 2024-03-28 20:28:33.000000 galarp-0.0.3/setup.py
+drwxrwsr-x   0 hsouchereau  (2478) hsouchereau  (2478)        0 2024-03-22 22:26:16.804611 galarp-1.0.0/
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)     1086 2024-03-22 22:25:26.000000 galarp-1.0.0/LICENSE
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)      825 2024-03-22 22:26:16.802790 galarp-1.0.0/PKG-INFO
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)       88 2024-03-22 22:25:23.000000 galarp-1.0.0/README.md
+drwxrwsr-x   0 hsouchereau  (2478) hsouchereau  (2478)        0 2024-03-22 22:26:16.708916 galarp-1.0.0/galarp/
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)      385 2024-03-21 15:25:04.000000 galarp-1.0.0/galarp/__init__.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     7515 2024-03-22 15:13:52.000000 galarp-1.0.0/galarp/particle_grids.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     4044 2024-03-22 14:02:51.000000 galarp-1.0.0/galarp/plotting.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     6698 2024-03-21 21:45:28.000000 galarp-1.0.0/galarp/rampressure.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     7692 2024-03-20 14:31:13.000000 galarp-1.0.0/galarp/shadows.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)      696 2024-03-12 15:41:42.000000 galarp-1.0.0/galarp/tests.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     6292 2024-03-22 15:08:46.000000 galarp-1.0.0/galarp/utils.py
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     5388 2024-03-20 17:22:14.000000 galarp-1.0.0/galarp/winds.py
+drwxrwsr-x   0 hsouchereau  (2478) hsouchereau  (2478)        0 2024-03-22 22:26:16.785212 galarp-1.0.0/galarp.egg-info/
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)      825 2024-03-22 22:26:16.000000 galarp-1.0.0/galarp.egg-info/PKG-INFO
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)      326 2024-03-22 22:26:16.000000 galarp-1.0.0/galarp.egg-info/SOURCES.txt
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)        1 2024-03-22 22:26:16.000000 galarp-1.0.0/galarp.egg-info/dependency_links.txt
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)       30 2024-03-22 22:26:16.000000 galarp-1.0.0/galarp.egg-info/requires.txt
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)        7 2024-03-22 22:26:16.000000 galarp-1.0.0/galarp.egg-info/top_level.txt
+-rw-rw-r--   0 hsouchereau  (2478) hsouchereau  (2478)       38 2024-03-22 22:26:16.805647 galarp-1.0.0/setup.cfg
+-rw-------   0 hsouchereau  (2478) hsouchereau  (2478)     1210 2024-03-22 22:26:12.000000 galarp-1.0.0/setup.py
```

### Comparing `galarp-0.0.3/LICENSE` & `galarp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galarp-0.0.3/galarp/particle_grids.py` & `galarp-1.0.0/galarp/particle_grids.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,280 +1,191 @@
+
 import numpy as np
 from astropy import units as u
 from matplotlib import pyplot as plt
 
-from .postprocessing.plotting import general_plots
 import gala.dynamics as gd
 from . import utils
 
 
 from tqdm import tqdm
 
 
-__all__ = [
-    "ParticleGrid",
-    "UniformGrid",
-    "ExponentialGrid",
-    "generate_exponential_positions",
-]
+__all__ = ["ParticleGrid", "UniformGrid", "ExponentialGrid", "generate_positions"]
 
 
 class ParticleGrid:
+
     def __init__(self, name="PG"):
-        self.container = []  # List of PhaseSpacePosition objects
+        self.container = []             # List of PhaseSpacePosition objects
         self.name = name
-
+    
     def generate(self):
-        raise NotImplementedError(
-            "This is an abstract class. Please use a \
-            subclass."
-        )
-
-    def plot_phase_space(self, ax=None, color="black", outname=None):
-        if ax is None:
-            fig, ax = plt.subplots(1, 2, facecolor="white", figsize=(8, 4))
+        raise NotImplementedError("This is an abstract class. Please use a subclass.")
+    
+    def plot_phase_space(self, ax, color="black", outname=None):
+        fig, ax = plt.subplots(1, 2, facecolor="white", figsize=(8, 4))
         for particle in self.container:
             ax[0].scatter(particle.x, particle.y, color=color)
             ax[1].scatter(particle.v_x, particle.v_y, color=color)
-
+        
         plt.tight_layout()
         if outname is not None:
             plt.savefig(outname, dpi=200)
         else:
             plt.show()
     
-    def get_xyz(self):
-        x, y, z = [], [], []
-        for particle in self.container:
-            x.append(particle.x.value)
-            y.append(particle.y.value)
-            z.append(particle.z.value)
-        return x, y, z
-
-
-    def plot_grid(self, **kwargs):
-        """ Plot the grid of particles in the xy and xz planes. """
-        particle_size = kwargs.get("particle_size", 1)
-        max_particles = kwargs.get("max_particles", 1000)
-
-        fig, ax = plt.subplots(1, 2, facecolor="white", figsize=(8, 4))
-        xs, ys, zs = self.get_xyz()
-
-        ax[0].scatter(xs, ys, color="black", s=particle_size)
-        ax[1].scatter(xs, zs, color="black", s=particle_size)
-        
-        ax[0].set_xlabel("x [kpc]")
-        ax[0].set_ylabel("y [kpc]")
-        ax[1].set_xlabel("x [kpc]")
-        ax[1].set_ylabel("z [kpc]")
-        
-        ax[0].set_xlim(-self.Rmax.value, self.Rmax.value)
-        ax[0].set_ylim(-self.Rmax.value, self.Rmax.value)
-        ax[1].set_xlim(-self.Rmax.value, self.Rmax.value)
-        ax[1].set_ylim(-self.Rmax.value, self.Rmax.value)
-
-        plt.tight_layout()
-        plt.show()
-    
-
-    def plot_density(self, gridsize=40, outname=None, **kwargs):
-        """ Generate hexbin plots of the x-y and x-z particle densities.
-
-        Args:
-            gridsize (int): Number of bins in the hexbin plots.
-            outname (str): Filename for saving the output plot. Will just run plt.show() if None.
-        """
-        general_plots.plot_density(self.get_xyz(), gridsize=gridsize, outname=outname,  **kwargs)
-
-
     def save(self, outname):
         utils.pickle_obj(self.container, outname)
 
 
+
 class UniformGrid(ParticleGrid):
-    """Class to initialize a grid of particles in the xy plane with circular
-    velocities based on a given gravitational potential.
+    """ Class to initialize a grid of particles in the xy plane with circular velocities based on a given gravitational potential.
 
-    Usage:
-        ```
-        mass_profile = gn.gen_mass_profile(potential)
-        grid = gn.ParticleGrid()
-        grid.generate(mass_profile)
-        ```
+        Usage:
+            ```
+            mass_profile = gn.gen_mass_profile(potential)
+            grid = gn.ParticleGrid()
+            grid.generate(mass_profile)
+            ```
     """
 
-    def __init__(self, Rmax=10, n_particles=50, z_start=0.0, veldisp=10.0):
-        """Generate a grid of particles in the xy plane with circular
-            velocities based on a given gravitational potential.
-            Can also include a Gaussian velocity dispersion (helpful for
-            including a scale height in the disk).
+    def __init__(self, Rmax=10, n_particles=50, z_start=0., veldisp=10.):
+        """ Generate a grid of particles in the xy plane with circular velocities based on a given gravitational potential.
+            Can also include a Gaussian velocity dispersion (helpful for including a scale height in the disk).
 
         Args:
-            mass_profile (interp1d): The mass profile of the potential in scipy
-            interp1d format. Defaults to None.
+            mass_profile (interp1d): The mass profile of the potential in scipy interp1d format. Defaults to None.
             Rmax (_type_): The maximum radius of the grid particles.
-            n_particles (int, optional): Number of particles between -Rmax and
-                Rmax. Defaults to 50.
-            z_start (float, optional): The z-level to initialize the grid in.
-                Defaults to 0.
+            n_particles (int, optional): Number of particles between -Rmax and Rmax. Defaults to 50.
+            z_start (float, optional): The z-level to initialize the grid in. 0 is . Defaults to 0.
             veldisp (float, optional): _description_. Defaults to 10.
-            velocities (bool, optional): If false, particles have no velocities.
-                Defaults to True.
+            velocities (bool, optional): If false, particles have no velocities. Defaults to True.
         """
-
+        
         super().__init__(name="UG")
-
+        
         self.Rmax = Rmax
         self.n_particles = n_particles
         self.z_start = z_start
         self.veldisp = veldisp
 
+    
     def generate(self, mass_profile, velocities=True):
         particle_range = np.linspace(-self.Rmax, self.Rmax, self.n_particles) * u.kpc
 
         for x in particle_range:
             for y in particle_range:
-                p_x0 = u.Quantity([x, y, self.z_start * u.kpc])
-                R = np.sqrt(x**2 + y**2)
+                p_x0 =  u.Quantity([x, y, self.z_start * u.kpc])
+                R = np.sqrt(x ** 2 + y **2)
                 if R > self.Rmax * u.kpc:
                     continue
-
+                
                 if velocities:
                     theta = np.arctan2(y, x)
-
-                    # Initialize with circular velocity
-                    p_v0 = utils.velocity(mass_profile, R, theta)
+                    
+                    p_v0 = utils.velocity(mass_profile, R, theta)          # Initialize with circular velocity
                     if self.veldisp is not None:
-                        # Add random velocity dispersion
-                        p_v0 += np.random.normal(scale=self.veldisp, size=3) * (
-                            u.km / u.s
-                        )
+                        p_v0 += np.random.normal(scale=self.veldisp, size=3) * (u.km / u.s)    # Add random velocity dispersion
                 else:
-                    p_v0 = [0.0, 0.0, 0.0] * (u.km / u.s)
-
+                    p_v0 = [0., 0., 0.] * (u.km / u.s)
+                
                 w0 = gd.PhaseSpacePosition(pos=p_x0, vel=p_v0.to(u.kpc / u.Myr))
                 self.container.append(w0)
+        
 
 
 class ExponentialGrid(ParticleGrid):
-    def __init__(
-        self,
-        h_R=4 * u.kpc,
-        h_z=0.5 * u.kpc,
-        n_particles=500,
-        veldisp=10.0 * u.km / u.s,
-        Rmax=None,
-        zmax=None,
-    ):
+    
+    def __init__(self, h_R=4 * u.kpc, h_z=0.5 * u.kpc, n_particles=500, veldisp=10. * u.km/u.s, Rmax = None, zmax=None):
         super().__init__(name="EG")
-
+        
         self.h_R = h_R
         self.h_z = h_z
-
+        
         self.Rmax = Rmax if Rmax is not None else self.h_R * 4
         self.zmax = zmax if zmax is not None else self.h_z * 4
-
+        
         self.n_particles = n_particles
         self.veldisp = veldisp
-
+    
+    
     def generate(self, mass_profile, velocities=True, positions=None):
-        if positions is None:  # Generate positions if nothing given
-            xs, ys, zs = generate_exponential_positions(
-                h_R=self.h_R,
-                h_z=self.h_z,
-                n_particles=self.n_particles,
-                Rmax=self.Rmax,
-                zmax=self.zmax,
-                outname=None,
-            )
-        elif isinstance(positions, str):    # If string assume this is a filename
+        
+        if positions is None:                       # Generate positions if nothing given
+            xs,ys,zs = generate_exponential_positions(h_R=self.h_R, h_z=self.h_z, n_particles=self.n_particles, 
+                                                      rmax=self.Rmax, zmax=self.zmax, outname=None)
+        elif type(positions) == str:                # If string assume this is a filename
             xs, ys, zs = self.load_positions(positions)
-        else:
+        else:                                       
             xs, ys, zs = positions
 
         # Create PhaseSpacePositions for all points, and initialize velocities
         for i in range(self.n_particles):
-            x, y, z = xs[i], ys[i], zs[i]
-
-            p_x0 = u.Quantity([x, y, z] * u.kpc)
-
-            R = np.sqrt(x**2 + y**2 + z**2) * u.kpc
-
+            x,y,z = xs[i], ys[i], zs[i]
+            
+            p_x0 =  u.Quantity([x, y, z] * u.kpc)
+            
+            R = np.sqrt(x ** 2 + y **2 + z**2) * u.kpc
+            
             if velocities:
                 theta = np.arctan2(y, x)
-                vx, vy = self.velocity(
-                    mass_profile, R, theta
-                )  # Initialize with circular velocity
-
+                vx, vy = self.velocity(mass_profile, R, theta)     # Initialize with circular velocity
+                
                 inc = np.arctan2(z, np.sqrt(x**2 + y**2))
                 vtot = np.sqrt(vx**2 + vy**2)
-                vz = (
-                    vtot * np.sin(inc)
-                )  # TODO improve this (better than nothing but not ideal. Leads to "sloshing")
-
+                vz = vtot * np.sin(inc)                            # TODO improve this (better than nothing but not ideal. Leads to "sloshing")
+                                
                 p_v0 = u.Quantity([vx, vy, vz])
-
+                
                 if self.veldisp is not None:
-                    p_v0 += np.random.normal(scale=self.veldisp.value, size=3) * (
-                        u.km / u.s
-                    )  # Add random velocity dispersion
+                    p_v0 += np.random.normal(scale=self.veldisp.value, size=3) * (u.km / u.s)    # Add random velocity dispersion
             else:
-                p_v0 = [0.0, 0.0, 0.0] * (u.km / u.s)
+                p_v0 = [0., 0., 0.] * (u.km / u.s)
 
             w0 = gd.PhaseSpacePosition(pos=p_x0, vel=p_v0.to(u.kpc / u.Myr))
             self.container.append(w0)
+    
 
     def load_positions(self, filename):
-        """Create the grid of particles from a file of positions (to save on time not needed to rerun the MC sim)
+        """ Create the grid of particles from a file of positions (to save on time not needed to rerun the MC sim)
         Args:
             filename (numpy savetxt file): Text file of positions
         """
         positions = np.load(filename)
         return positions
-
-    def velocity(self, mass_profile, R, theta):
-        """ Get the velocity of a particle in the xy plane given an angle and the mass profile
+    
+            
         
-        Args:
-            mass_profile (interp1d): The mass profile of the potential in scipy interp1d format.
-            R (float): The radius of the particle.
-            theta (float): The angle of the particle.
-        """
-        vx = -utils.v_circ(mass_profile(R) * u.M_sun, R) * np.sin(theta)
-        vy = utils.v_circ(mass_profile(R) * u.M_sun, R) * np.cos(theta)
+    def velocity(self, mass_profile, R, theta):
+        vx = - utils.v_circ(mass_profile(R) * u.M_sun, R) * np.sin(theta)
+        vy =   utils.v_circ(mass_profile(R) * u.M_sun, R) * np.cos(theta)
         return vx, vy
 
 
-def generate_exponential_positions(
-    n_particles,
-    h_R=4 * u.kpc,
-    h_z=0.5 * u.kpc,
-    Rmax=15 * u.kpc,
-    zmax=2 * u.kpc,
-    outname=None,
-):
+
+def generate_exponential_positions(self, n_particles,  h_R = 4*u.kpc, h_z = 0.5*u.kpc, rmax=15 * u.kpc, zmax=2 * u.kpc, outname=None):
     def remap(value, a, b):
         return (value * (b - a)) + a
+    
+    n_0 = 1 / (4 * np.pi * h_R**2 * h_z).value  # This normalizes the probability distribution
 
-    n_0 = (
-        1 / (4 * np.pi * h_R**2 * h_z).value
-    )  # This normalizes the probability distribution
-
-    h_R, h_z = h_R.to(u.kpc).value, h_z.to(u.kpc).value
-    rmax = Rmax.to(u.kpc).value
-    zmax = zmax.to(u.kpc).value
+    h_R, h_z = self.h_R.to(u.kpc).value, self.h_z.to(u.kpc).value
+    rmax = self.Rmax.to(u.kpc).value
+    zmax = self.zmax.to(u.kpc).value
 
     Rs = []
     zs = []
 
     for n in tqdm(range(n_particles)):
         good = False
-        while not good:  # TODO maybe add a max_tries here with a warning message
+        while not good:     # TODO maybe add a max_tries here with a warning message
             rand_R, rand_z = np.random.random(2)
-            R, z = remap(rand_R, 0, rmax), remap(rand_z, -zmax, zmax)
+            R,z = remap(rand_R, 0, rmax), remap(rand_z, -zmax, zmax)
 
             v = n_0 * np.exp(-R / h_R) * np.exp(-np.abs(z) / h_z)
 
             if np.random.random() <= v:
                 Rs.append(R)
                 zs.append(z)
```

### Comparing `galarp-0.0.3/galarp/rampressure.py` & `galarp-1.0.0/galarp/rampressure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,245 +1,195 @@
-"""Classes for implementing orbits under ram pressure acceleration."""
+""" Classes for implementing orbits under ram pressure acceleration. """
 
 # Third Party
 import os
 import pickle
 import astropy.units as u
+from astropy.units import Quantity
 import numpy as np
 
 from tqdm import tqdm
 
-from .postprocessing import utils
+from matplotlib import pyplot as plt
 
 # This module
-from . import shadows, winds
+from . import plotting, shadows, utils, winds
 
 import gala.dynamics as gd
+import gala.potential as gp
 from gala.units import galactic
 
 
-# import integrate as gi            # If debugging
+#import integrate as gi            # If debugging
 import gala.integrate as gi
 
 
-__all__ = ["F_RPS_constant_wind", "RPSim", "OrbitContainer"]
 
+__all__ = ['F_RPS_constant_wind', 'RPSim', "OrbitContainer"]
 
-def F_RPS_constant_wind(
-    t, w, potential, shadow, wind, rho, r_cloud, m_cloud, wind_on=True, debug=False
-):
+
+
+def F_RPS_constant_wind(t, w, potential, shadow, wind, rho, r_cloud, m_cloud, wind_on=True, debug=False):
     # position units are in kpc
     # velocity units here are in kpc/Myr
     x, y, z, vx, vy, vz = w
     q = np.stack((x, y, z), axis=1)
     p = np.stack((vx, vy, vz), axis=1)
 
     # compute acceleration from potential:
-    _t = np.array([0.0])
+    _t = np.array([0.])
     acc = -potential._gradient(q, _t).T
-
+    
     # Compute acceleration from ram pressure
-    # a_ram = pi * rho * v_perp^2 * r_cloud^2 / m_cloud
+    # a_ram = pi * rho * v_perp^2 * r_cloud^2 / m_cloud 
     # TODO remove units altogether
     if wind_on:
         v_perp = p - wind.evaluate(t)
-        a_ram = (np.pi * rho.evaluate(t) * r_cloud**2 / m_cloud).to(1 / u.kpc).value * (
-            v_perp**2
-        )
-
+        a_ram = (np.pi * rho.evaluate(t) * r_cloud **2 / m_cloud).to(1/u.kpc).value * (v_perp ** 2)
+        
         a_ram = a_ram.T
 
         # If wind is on and shadow exists, apply shadow to appropriate particles
         if shadow is not None:
             shadow = shadow.evaluate(q, t).T
             a_ram *= shadow
 
         acc += a_ram
-
+    
     return np.vstack((p.T, acc))
 
 
 class RPSim:
-    def __init__(
-        self,
-        wind,
-        potential,
-        rho_icm=None,
-        shadow=None,
-        potential_name="",
-        method=F_RPS_constant_wind,
-    ):
+    def __init__(self, wind, potential, rho_icm=None, shadow=None, potential_name="", method=F_RPS_constant_wind):
         self.method = method
-
+        
         self.wind = wind
         self.potential = potential
-
+        
         self.shadow = shadow
 
         self.potential_name = potential_name
-
+        
         self.rho_icm = rho_icm
 
         self.inclination = wind.inclination()
-        if (
-            np.rad2deg(self.inclination) < 10
-            and type(self.shadow) != shadows.EdgeOnShadow
-        ):
-            print(
-                "Warning: Inclination is less than 10 degrees. You should be using an EdgeOnShadow."
-            )
-
+        if np.rad2deg(self.inclination) < 10 and type(self.shadow) != shadows.EdgeOnShadow:
+            print("Warning: Inclination is less than 10 degrees. You should be using an EdgeOnShadow.")
+        
         self.sim_results = []
 
-    def run(
-        self,
-        particles,
-        rho_icm=2e-27 * (u.g / u.cm**3),
-        t0=100 * u.Myr,
-        r_cloud=50 * u.pc,
-        m_cloud=1e5 * u.Msun,
-        wind_on=True,
-        integration_time=500 * u.Myr,
-        dt=5 * u.Myr,
-        printout=True,
-        wind=None,
-        outdir=None,
-        debug=False,
-    ):
+
+    def run(self, particles,
+            rho_icm=2e-27 * (u.g / u.cm**3), 
+            t0 = 100 * u.Myr, r_cloud = 50 * u.pc, m_cloud = 1e5 * u.Msun,
+            wind_on = True,
+            integration_time = 500 * u.Myr, dt = 5 * u.Myr,
+            printout=True,
+            wind=None,
+            outdir=None, debug=False):
+
+        wind_vector = self.wind.vector.to(u.kpc / u.Myr).value
 
         if type(rho_icm) is u.Quantity:
             self.rho_icm = winds.Density(rho_icm)
-
+        
         # Allow for user to switch out wind in the run method
         if wind is not None:
             self.wind = wind
 
         if printout:
             printout_width = 80
             print("".center(printout_width, "-"))
-            print(
-                f" Running GALA sim with  {self.wind.wind_strength():.2e}  wind at  {self.wind.inclination():.2f}  degrees ".center(
-                    printout_width, "-"
-                )
-            )
-            print(
-                f" Running for {integration_time}  at a timestep of  {dt}  ({integration_time / dt:.1f} steps) ".center(
-                    printout_width, "-"
-                )
-            )
+            print(f' Running GALA sim with  {self.wind.wind_strength():.2e}  wind at  {self.wind.inclination():.2f}  degrees '.center(printout_width, "-"))
+            print(f' Running for {integration_time}  at a timestep of  {dt}  ({integration_time / dt:.1f} steps) '.center(printout_width, "-"))
             print("".center(printout_width, "-"))
-            print(
-                f" Container contains {len(particles.container)} particles ".center(
-                    printout_width, "-"
-                )
-            )
-            print(
-                f" Each cloud has a mass of  {m_cloud.value:.1e} solar masses  and a radius of  {r_cloud:.2f}   ".center(
-                    printout_width, "-"
-                )
-            )
-            print(
-                f" This corresponds to a density of {(m_cloud / r_cloud **3).to(u.g/u.cm**3):.2e}   ".center(
-                    printout_width, "-"
-                )
-            )
+            print(f' Container contains {len(particles.container)} particles '.center(printout_width, "-"))
+            print(f' Each cloud has a mass of  {m_cloud.value:.1e} solar masses  and a radius of  {r_cloud:.2f}   '.center(printout_width, "-"))
+            print(f' This corresponds to a density of {(m_cloud / r_cloud **3).to(u.g/u.cm**3):.2e}   '.center(printout_width, "-"))
             print("".center(printout_width, "-"))
 
         # potential, shadow, wind_vec, rho, r_cloud, m_cloud, damping=1, wind_on=True)
-
-        integrator = gi.RK5Integrator(
-            self.method,
-            func_args=(
-                self.potential,
-                self.shadow,
-                self.wind,
-                self.rho_icm,
-                r_cloud,
-                m_cloud,
-                wind_on,
-            ),
-            func_units=galactic,
-            progress=not debug,
-        )
-
+    
+        integrator = gi.RK5Integrator(self.method,
+                                           func_args=(self.potential, 
+                                                      self.shadow,
+                                                      self.wind, 
+                                                      self.rho_icm,
+                                                      r_cloud, 
+                                                      m_cloud,
+                                                      wind_on),
+                                           func_units=galactic,
+                                           progress=not debug)
+        
         if debug:
             for p in tqdm(particles):
-                orbit = integrator.run(
-                    gd.combine(particles.container), dt=dt, t1=0, t2=integration_time
-                )
+                orbit = integrator.run(gd.combine(particles.container), dt=dt, t1=0, t2=integration_time)
             return
-
-        orbits = integrator.run(
-            gd.combine(particles.container), dt=dt, t1=0, t2=integration_time
-        )
+            
+        orbits = integrator.run(gd.combine(particles.container), dt=dt, t1=0, t2=integration_time)
         self.sim_results.append(orbits)
 
-        metadata = {
-            "WIND": self.wind,
-            "POTENTIAL": self.potential,
-            "POTENTIAL_NAME": self.potential_name,
-            "SHADOW": self.shadow,
-            "RHO_ICM": self.rho_icm,
-            "PARTICLE_GRID": particles,
-            "R_CLOUD": r_cloud,
-            "M_CLOUD": m_cloud,
-            "WIND_ON": wind_on,
-            "INTEGRATION_TIME": integration_time,
-            "DT": dt,
-        }
-
+        metadata = {"WIND": self.wind, "POTENTIAL": self.potential, "POTENTIAL_NAME": self.potential_name, "SHADOW": self.shadow, "RHO_ICM": self.rho_icm,
+                    "PARTICLE_GRID": particles,
+                    "R_CLOUD": r_cloud, "M_CLOUD": m_cloud, "WIND_ON": wind_on, "INTEGRATION_TIME": integration_time, "DT": dt}
+        
+                
         out = OrbitContainer(orbits, units=galactic, metadata=metadata)
-
+        
+        
         if outdir is not None:
             os.makedirs(outdir, exist_ok=True)
             save_orbits(out, outdir=outdir)
-
+        
         return out
 
+
     def __repr__(self) -> str:
-        return f"Ram Pressure Sim \n Wind: \t\t{self.wind.__repr__()}\n Shadow: \t{self.shadow.__repr__()}\n Potential: \t{self.potential}"
+        return f'Ram Pressure Sim \n Wind: \t\t{self.wind.__repr__()}\n Shadow: \t{self.shadow.__repr__()}\n Potential: \t{self.potential}'            
+
 
+def autogen_fn(md,  suffix="orbits"):
 
-def autogen_fn(md, suffix="orbits"):
     fn = ""
 
     if md["POTENTIAL_NAME"] != "":
         fn += f'{md["POTENTIAL_NAME"]}_'
     if md["WIND"] is not None:
         wind = md["WIND"]
-        fn += f"WIND_{wind.wind_strength().to(u.km/u.s).value:.0f}_{np.rad2deg(wind.inclination()):.0f}_"
+        fn += f'WIND_{wind.wind_strength().to(u.km/u.s).value:.0f}_{np.rad2deg(wind.inclination()):.0f}_'
     if md["SHADOW"] is not None:
         shadow = md["SHADOW"]
-        fn += f"_{shadow.shadow_name}_{shadow.damping}DAMP_"
+        fn += f'_{shadow.shadow_name}_{shadow.damping}DAMP_'
     fn += f'{md["M_CLOUD"].value:.0e}Msun_{md["R_CLOUD"].value:.0f}pc'
 
-    fn += f".{suffix}"
+    fn += f'.{suffix}'
 
     return fn
 
 
 def save_orbits(orbits, name="auto", outdir=""):
     metadata = orbits.metadata
     if name == "auto":
         name = autogen_fn(metadata)
 
-    with open(outdir + name, "wb") as f:
+    with open(outdir + name, 'wb') as f:
         pickle.dump(orbits, f)
-
+    
+    
 
 class OrbitContainer:
-    """ Container for storing orbits and metadata from a completed GalaRP run.
-    """
+
     def __init__(self, data, units=None, metadata={}):
         self.data = data
         self.units = units
 
         self.metadata = metadata
-
+        
+    
+    
     def plot(self, plot_3d=False, plot_orbits=False):
+        
         if plot_3d:
-            utils.k3d_plot([self])
-
+            plotting.k3d_plot([self])
+    
         if plot_orbits:
-            utils.plot_orbits(
-                self.data, wind=self.metadata["WIND"], shadow=self.metadata["SHADOW"]
-            )
+            plotting.plot_orbits(self.data, wind=self.metadata["WIND"], shadow=self.metadata["SHADOW"])
```

### Comparing `galarp-0.0.3/galarp/shadows.py` & `galarp-1.0.0/galarp/shadows.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,17 +49,15 @@
         Initializes an angled shadow from a wind object.
 
         Parameters:
         - wind (Wind): The wind object from which to initialize the shadow.
         """
         self.phi = wind.inclination()
 
-    def plot_shadow(
-        self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=0
-    ):
+    def plot_shadow(self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=0):
         """
         Plots the shadow on the given axes.
 
         Parameters:
         - ax (array-like, optional): The axes on which to plot the shadow. If not provided, a new figure will be created.
         - wind (Wind, optional): The wind object to plot along with the shadow.
         - color (str, optional): The color of the shadow.
@@ -67,70 +65,51 @@
         - x0, y0, z0 (float, optional): The coordinates of the origin of the shadow.
 
         Returns:
         - None
         """
         R_disk = self.R_disk.value if type(self.R_disk) is u.Quantity else self.R_disk
         R_plot = R_disk * 1.5
-
+        
         # Create figure if ax is not provided
         if ax is None:
             fig, ax = plt.subplots(1, 3, facecolor="white", figsize=(12, 4))
-
+        
         for axis in ax.flatten():
             axis.set_xlim(-R_plot, R_plot)
             axis.set_ylim(-R_plot, R_plot)
 
         x = np.linspace(-R_disk, R_disk, 100)
         y = np.linspace(-R_disk, R_disk, 100)
         X, Y = np.meshgrid(x, y)
         XY = self.evaluate(np.array([X, Y, np.zeros(X.shape) + z0]).T)
-        XZ = self.evaluate(np.array([X, np.zeros(X.shape) + y0, Y]).T)
-        YZ = self.evaluate(np.array([np.zeros(X.shape) + x0, X, Y]).T)
+        XZ = self.evaluate(np.array([X, np.zeros(X.shape) + y0, Y]).T)   
+        YZ = self.evaluate(np.array([np.zeros(X.shape) + x0, X, Y]).T)   
 
-        im1 = ax[0].imshow(
-            1 - XY,
-            origin="lower",
-            cmap="Greys",
-            alpha=0.5,
-            extent=(-R_disk, R_disk, -R_disk, R_disk),
-        )
-        im2 = ax[1].imshow(
-            1 - XZ,
-            origin="lower",
-            cmap="Greys",
-            alpha=0.5,
-            extent=(-R_disk, R_disk, -R_disk, R_disk),
-        )
-        im3 = ax[2].imshow(
-            1 - YZ,
-            origin="lower",
-            cmap="Greys",
-            alpha=0.5,
-            extent=(-R_disk, R_disk, -R_disk, R_disk),
-        )
+        im1 = ax[0].imshow(1- XY, origin="lower", cmap="Greys", alpha=0.5, extent=(-R_disk, R_disk, -R_disk, R_disk))
+        im2 = ax[1].imshow(1 - XZ, origin="lower", cmap="Greys", alpha=0.5, extent=(-R_disk, R_disk, -R_disk, R_disk))
+        im3 = ax[2].imshow(1 - YZ, origin="lower", cmap="Greys", alpha=0.5, extent=(-R_disk, R_disk, -R_disk, R_disk))
 
         plt.colorbar(mappable=im1, ax=ax[0], location="top")
         plt.colorbar(mappable=im2, ax=ax[1], location="top")
         plt.colorbar(mappable=im3, ax=ax[2], location="top")
 
         utils.plot_disk(ax, R_disk, lw=1, color="black")
 
         if wind is not None:
-            utils.plot_wind_vector(
-                wind.normalized().value, ax, length=0.5, loc=(-R_disk, -R_disk, -R_disk)
-            )
+            utils.plot_wind_vector(wind.normalized().value, ax, length=0.5, loc=(-R_disk, -R_disk, -R_disk))
 
         if ax is None:
             plt.tight_layout()
             if outname is not None:
                 plt.savefig(outname, dpi=200)
             else:
                 plt.show()
 
+
     def __repr__(self):
         """
         Returns a string representation of the shadow object.
 
         Returns:
         - repr (str): The string representation of the shadow object.
         """
@@ -144,96 +123,82 @@
 
     Args:
         damping (float, optional): The damping factor. Defaults to 0.5.
         R_disk (Quantity, optional): The radius of the disk. Defaults to 10 kpc.
         zmin (Quantity, optional): The minimum value of z above the disk. Defaults to 0 kpc.
         phi (float, optional): The angle in radians. Defaults to 20 degrees.
     """
-
-    def __init__(
-        self, damping=0.5, R_disk=10 * u.kpc, zmin=0 * u.kpc, phi=np.deg2rad(20)
-    ):
+    def __init__(self, damping=0.5, R_disk=10 * u.kpc, zmin=0 * u.kpc, phi=np.deg2rad(20)):
         super().__init__(damping=damping, R_disk=R_disk, shadow_name="Uniform")
         self.zmin, self.phi = zmin, phi
 
     def evaluate(self, q, t):
         x, y, z = q.T
 
         cent = _shadow_tangent(z, self.phi)
         dist = np.sqrt((x - cent) ** 2 + y**2)
 
         out = np.ones(dist.shape)
         in_disk = np.logical_and((z > self.zmin.value), (dist < self.R_disk.value))
         out[in_disk] = self.damping
         return out
 
-    def plot_shadow(
-        self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=None
-    ):
+    def plot_shadow(self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=None):
         z0 = self.zmin + 0.5 * u.kpc if z0 is None else z0
-        super().plot_shadow(
-            ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0=z0
-        )
+        super().plot_shadow(ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0 = z0)
 
 
 class ExponentialShadow(ShadowBase):
     """A class representing an exponential drop-off angled shadow.
 
     This class inherits from the ShadowBase class.
 
     Args:
         damping (float, optional): The damping factor. Defaults to 0.5.
         R_disk (Quantity, optional): The radius of the disk. Defaults to 10 kpc.
         zmin (Quantity, optional): The minimum value of z above the disk. Defaults to 0 kpc.
         phi (float, optional): The angle in radians. Defaults to 20 degrees.
     """
-
-    def __init__(
-        self, damping=0.5, R_disk=10 * u.kpc, zmin=0 * u.kpc, phi=np.deg2rad(20)
-    ):
+    def __init__(self, damping=0.5, R_disk=10 * u.kpc, zmin=0 * u.kpc, phi=np.deg2rad(20)):
         super().__init__(damping=damping, R_disk=R_disk, shadow_name="Exponential")
         self.zmin, self.phi = zmin, phi
 
     def evaluate(self, q, t):
         x, y, z = q.T
         cent = _shadow_tangent(z, self.phi)
         dist = np.sqrt((x - cent) ** 2 + y**2)
         out = np.exp(-dist / self.R_disk.value)
         in_disk = np.logical_and((z > self.zmin.value), (dist < self.R_disk.value))
-        out[in_disk] *= self.damping
+        out[in_disk] *= self.damping 
         return out
-
-    def plot_shadow(
-        self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=None
-    ):
+    
+    def plot_shadow(self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=None):
         z0 = self.zmin + 0.5 * u.kpc if z0 is None else z0
-        super().plot_shadow(
-            ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0=z0
-        )
+        super().plot_shadow(ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0 = z0)
 
 
 class EdgeOnShadow(ShadowBase):
+
     def __init__(self, damping=0.5, R_disk=10 * u.kpc, Z_disk=2 * u.kpc, x0=0 * u.kpc):
         super().__init__(damping=damping, R_disk=R_disk, shadow_name="EdgeOn")
 
         # Always assume kpc for xyz inputs (galactic coordinate system)
         self.x0 = x0.to(u.kpc).value
-        self.R_disk = R_disk.to(u.kpc).value
+        self.R_disk = R_disk.to(u.kpc).value        
         self.Z_disk = Z_disk.to(u.kpc).value
-
+        
     def evaluate(self, q, t):
         x, y, z = q.T
 
-        in_ellipsoid = (y / self.R_disk) ** 2 + (z / self.Z_disk) ** 2 < 1
+        in_ellipsoid = ((y / self.R_disk)) ** 2 + ((z / self.Z_disk)) ** 2 < 1
+
 
         out = np.ones(x.shape)
 
         out[np.logical_and((x >= 0), in_ellipsoid)] = self.damping
 
         return out
 
-    def plot_shadow(
-        self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=0
-    ):
-        super().plot_shadow(
-            ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0=z0
-        )
+    def plot_shadow(self, ax=None, wind=None, color="black", outname=None, x0=0, y0=0, z0=0):
+        super().plot_shadow(ax=ax, wind=wind, color=color, outname=outname, x0=z0, y0=y0, z0 = z0)
+
+
```

### Comparing `galarp-0.0.3/galarp/tests.py` & `galarp-1.0.0/galarp/tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 
 # Third Party
 import os
 import numpy as np
 
 
 # This module
-import galarp as grp
+import nonconserved as gn
+from . import utils
 
 from gala.units import galactic
 import astropy.units as u
 
 
 __all__ = ["test_uniform_shadow"]
 
 
-def test_uniform_shadow(plot_dir="plots/shadow_tests/"):
-    """Test that the angled shadows being created are correct"""
+def test_uniform_shadow(plot_dir = "plots/shadow_tests/"):
+    """ Test that the angled shadows being created are correct """
 
     os.makedirs(plot_dir, exist_ok=True)
 
     for angle in range(10, 90, 10):
-        wind = grp.RPWind(units=galactic)
-        wind.init_from_inc(np.deg2rad(angle), 300 * u.km / u.s)
-
-        shadow = grp.UniformShadow()
+        wind = gn.RPWind(units=galactic)
+        wind.init_from_inc(np.deg2rad(angle), 300 * u.km  / u.s)
+        
+        shadow = gn.UniformShadow()
         shadow.init_from_wind(wind)
         shadow.plot_shadow(wind=wind, outname=f"{plot_dir}shadow_{angle}.pdf")
+
```

### Comparing `galarp-0.0.3/galarp/winds.py` & `galarp-1.0.0/galarp/winds.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,44 @@
-
-from astropy.table import Table
+# Third Party
+import os
+import pickle
 import astropy.units as u
 from astropy.units import Quantity
 import numpy as np
 
-from scipy.interpolate import interp1d
+from tqdm import tqdm
+
+from matplotlib import pyplot as plt
+
+# This module
+from . import shadows, utils
+
+import gala.dynamics as gd
+import gala.potential as gp
+from gala.units import galactic
+
+
+#import integrate as gi            # If debugging
+import gala.integrate as gi
 
 
+__all__ = ['RPWind', 'LorentzianWind', 'StepFunctionWind', 'Density', 'ExponentialDensity', 'InterpolatedDensity']
 
-__all__ = [
-    "RPWind",
-    "LorentzianWind",
-    "StepFunctionWind",
-    "InterpolatedWind",
-    "Density",
-    "ExponentialDensity",
-    "InterpolatedDensity",
-]
 
 
 class RPWind:
-    """Class to represent a ram pressure wind
+    """ Class to represent a ram pressure wind
 
-    Usage:
-        ```
-        wind = gn.RPWind([50, 0, 50] * (u.km / u.s), units=gn.galactic)  # Initializes a wind at 45 degrees in the x-z plane.
-
-        wind = gn.RPWind(units=galactic)                                 # Achieves the same thing.
-        wind.init_from_inc(np.deg2rad(45), 100 * u.km  / u.s)
-        ```
+        Usage:
+            ```
+            wind = gn.RPWind([50, 0, 50] * (u.km / u.s), units=gn.galactic)  # Initializes a wind at 45 degrees in the x-z plane.
+
+            wind = gn.RPWind(units=galactic)                                 # Achieves the same thing.
+            wind.init_from_inc(np.deg2rad(45), 100 * u.km  / u.s)          
+            ```
     """
 
     def __init__(self, vector=None, units=None):
         """
         Args:
             vector (astropy Quantity, optional): Wind vector. Can also be initialized using self.init_from_inc(). Defaults to None.
             units (_type_, optional): _description_. Defaults to None.
@@ -42,168 +48,117 @@
         # self.vector = Quantity(vector)
 
         self.units = units
         if self.units is not None:
             if type(self.vector) == Quantity:
                 self.vector = self.vector.to(self.units["length"] / self.units["time"])
             else:
-                self.vector *= self.units["length"] / self.units["time"]
+                self.vector *= (self.units["length"] / self.units["time"])
 
     def evaluate(self, t):
-        """Return the wind vector at time t. For the default wind vector, this is JUST the vector converted to kpc/Myr"""
+        """ Return the wind vector at time t. For the default wind vector, this is JUST the vector converted to kpc/Myr """
         return self.vector.to(u.kpc / u.Myr).value
 
     def initialize_vector(self):
         if self.units is not None:
             self.vector = self.vector.to(self.units["length"] / self.units["time"])
 
     def init_from_inc(self, inclination, strength):
-        """Initialize the wind vector from an inclination and strength"""
-
+        """ Initialize the wind vector from an inclination and strength """
         x = strength * np.cos(inclination)
         z = strength * np.sin(inclination)
-        self.vector = Quantity([x, 0 * x.unit, z]).to(
-            self.units["length"] / self.units["time"]
-        )
+        self.vector = Quantity([x, 0 * x.unit, z]).to(self.units["length"] / self.units["time"])
 
     def wind_strength(self):
-        """Return the length (strength) of the wind vector"""
-        return np.sqrt(sum(self.vector**2))
+        """ Return the length (strength) of the wind vector """
+        return np.sqrt(sum(self.vector ** 2))
 
     def normalized(self):
-        """Return the normalized wind vector"""
+        """ Return the normalized wind vector """
         return self.vector / self.wind_strength()
-
+    
     def vector_to_units(self, units):
         return self.vector.to(units)
-
+    
     def vector_as_value(self):
         if type(self.vector) == Quantity:
             return self.vector.value
         else:
             return self.vector
 
     def inclination(self):
-        x, y, z = self.vector_as_value()
+        x,y,z = self.vector_as_value()
         return np.arctan2(z, np.sqrt(x**2 + y**2))
-
+    
     def __repr__(self):
         return f"<RP Wind Vector={self.vector}  Inclination={np.round(np.rad2deg(self.inclination()), 2):.2f}  >"
 
 
 class LorentzianWind(RPWind):
-    """Ram pressure wind that is damped by a Lorentzian profile.
+    """ Ram pressure wind that is damped by a Lorentzian profile. 
         Reaches max (which is just the unadjusted RP wind value) at t0.
 
     Args:
         gn (_type_): _description_
     """
-
     def __init__(self, t0=0 * u.Myr, width=200 * u.Myr, **kwargs):
         super().__init__(**kwargs)
-        self.t0 = t0.to(u.Myr).value  # Units are in Myr
-        self.width = width.to(u.Myr).value  # Units are in Myr
-
+        self.t0 = t0.to(u.Myr).value                 # Units are in Myr
+        self.width = width.to(u.Myr).value              # Units are in Myr
+        
     def evaluate(self, t):
-        """Return the wind vector damped by a Lorentzian profile"""
-        return super().evaluate(t) * 1 / ((2 * (t - self.t0) / self.width) ** 2 + 1)
+        """ Return the wind vector damped by a Lorentzian profile """
+        return super().evaluate(t) * 1 / ((2 * (t - self.t0) / self.width)**2 + 1)
 
 
 class StepFunctionWind(RPWind):
-    """A wind represented by a step function (no wind immediately into full wind at time t0)
-    Good for testing that time variability is working.
+    """ A wind represented by a step function (no wind immediately into full wind at time t0)
+        Good for testing that time variability is working.
 
     """
-
     def __init__(self, t0=0 * u.Myr, **kwargs):
         super().__init__(**kwargs)
         self.t0 = t0.to(u.Myr).value
-
+    
     def evaluate(self, t):
         factor = t > self.t0
         return super().evaluate(t) * factor
-    
-
-class InterpolatedWind(RPWind):
-    """ Wind class that returns an interpolated value for the wind vector at a given time t based on a scipy 
-        interp1D object.
-
-    """
-    def __init__(self, interp=None, inc=np.deg2rad(90), **kwargs):
-        super().__init__(**kwargs)
-        self.inc = inc
-        self.vector = kwargs.get('vector', u.Quantity([np.cos(inc), 0, np.sin(inc)]) * u.km/u.s)
 
-        self.interp = interp
-
-        self.unit_vector = self.vector / np.linalg.norm(self.vector)
-        print(self.unit_vector)
-
-
-    def evaluate(self, t):
-        return self.unit_vector * self.interp(t)
     
-
-    def from_xy(self, xs, ys):
-        self.interp = interp1d(xs, ys, bounds_error=False, fill_value='extrapolate')
-
-    @staticmethod
-    def from_table(fn, time_key, vel_keys, format='ascii', verbose=False, v_format=u.cm/u.s, ts_format=u.s, 
-                   **kwargs):
-        t = Table.read(fn, format=format)
-
-        if verbose:
-            print(f'Loaded Table with {len(t)} rows, and keys: {t.keys()}')
-
-        ts = t[time_key] * ts_format.to(u.Myr)
-
-        if not isinstance(vel_keys, list): 
-            vel_keys = [vel_keys]
-
-        vels = np.array([t[key] for key in vel_keys])
-        v_tot = np.sqrt(np.sum(vels**2, axis=0)) * v_format
-        
-        interp = interp1d(ts, v_tot, bounds_error=False, fill_value='extrapolate')
-
-        return InterpolatedWind(interp=interp, **kwargs)
-
-
-
 class Density:
-    """Parent class to represent time-variable densities."""
-
+    """ Parent class to represent time-variable densities. 
+    """
     def __init__(self, rho):
         self.rho = rho
         assert type(rho) == u.Quantity, "Density must be a Quantity"
 
     def evaluate(self, t):
         return self.rho.to(u.g / u.cm**3)
-
+    
 
 class ExponentialDensity(Density):
     def __init__(self, rho, t0, width):
         super().__init__(rho)
         self.t0 = t0
         self.width = width
 
         assert type(t0) == u.Quantity, "t0 must be a Quantity"
         assert type(width) == u.Quantity, "width must be a Quantity"
 
     def evaluate(self, t):
-        return self.rho * np.exp(-(((t - self.t0) / self.width) ** 2))
-
+        return self.rho * np.exp(-((t - self.t0) / self.width) ** 2)
+    
 
 class InterpolatedDensity(Density):
-    """Density class that returns an interpolated value for the density at a given time t.
-    Helpful for if you are determining the density through a GALA orbit and want it to be as realistic
-    as possible.
+    """ Density class that returns an interpolated value for the density at a given time t.
+        Helpful for if you are determining the density through a GALA orbit and want it to be as realistic
+        as possible.
     """
+    def __init__(self, rho_interp):
+        super().__init__(0)         # The "rho" can just be 0 here, as it will be overwritten by the interpolation
 
-    def __init__(self, interp):
-        super().__init__(
-            0
-        )  # The "rho" can just be 0 here, as it will be overwritten by the interpolation
-
-        self.interp = interp
+        self.rho_interp = rho_interp
+        
 
     def evaluate(self, t):
-        return self.interp(t)
+        return np.interp(t, self.t, self.values)
+
```

### Comparing `galarp-0.0.3/setup.py` & `galarp-1.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 
 #!/usr/bin/env python
 # Licensed under an MIT license - see LICENSE
 
-from galarp import __version__
+import os
+import sys
 
 
 from setuptools import setup, find_packages
 
 
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.rst").read_text()
+long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='galarp',
-    version=__version__,
+    version='1.0.0',
     author='Harrison Souchereau',
     author_email='harrison.souchereau@yale.edu',
     description='A ram pressure add-on for Gala numerical integration of gravitational potentials',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/HSouch/galarp',
+    url='https://github.com/your-username/your-package-repo',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

