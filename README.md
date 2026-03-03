# LCEM-Setup
## Legacy console edition minecraft
The required steps to run your very own iteration of LCEM from source.

prerequisites:
- obtain the `2gb` .rar from trusted source.

---
> [!NOTE]
> https://archive.org/details/vs-2012-rc-ult-enu
> Open the solution with `Visual Studio 2012` using 'Visual c++ profile'

> [!NOTE]
> in `Windows64_Minecraft.cpp`:
> comment out: `createDeviceFlags |= D3D11_CREATE_DEVICE_DEBUG;`

> [!WARNING]
> Make sure speakers are plugged in, will possibly crash otherwise.

> [!NOTE]
> Select Windows64 solution platform and run with local windows debugger

> [!NOTE]
> Select & right click `Minecraft.Client` from within the project, set as startup project.

> [!TIP]
> Game should launch.
> Only gamepad controls.
> Possible shim with: https://github.com/LCEMP/LCEMP/

---
> [!CAUTION]
> Might crash because of `SoundTypes.h`
> There is a duplicate file under `Minecraft.Client`, remove duplicate and re-compile.
