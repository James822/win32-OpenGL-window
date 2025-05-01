# win32/OpenGL window

Code for a simple win32/wgl window with an OpenGL context. See my [blog post](https://james822.github.io/posts/win32_window_opengl.html) for a tutorial on how to write this yourself.


## BUILD INSTRUCTIONS

You'll need to a few things to be able to compile this example with MSVC. See my blog post for more details.

Firstly, you need to install the Build Tools for Visual Studio from this link: [https://james822.github.io/posts/win32_window_opengl.html](https://james822.github.io/posts/win32_window_opengl.html). Make sure you select the "Desktop development with C++" package.

Either use a `vcvars<>.bat` file to configure a CMD for building with MSVC, or use a developer command prompt. The location of both of these are dependent, but I found mine in the `C:\Program Files (x86)\Microsoft Visual Studio\2022\BuildTools\VC\Auxiliary\Build` folder for the vcvars file, or the `C:\Program Files (x86)\Microsoft Visual Studio\2022\BuildTools\Common7\Tools` folder for the developer command prompt location.

If you want to compile with Visual Studio IDE, then simply open the project in a solution and do so, but you'll need to specify the extra flags for compiling and linking.

Once this is done, you can compile with:

`cl User32.lib Gdi32.lib Opengl32.lib win32_window.c`

And the output file should be `win32_window.exe`


While the exe is running, hit the `ESC` key anytime to exit the application.


