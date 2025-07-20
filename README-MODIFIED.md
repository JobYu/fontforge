# FontForge 20250720-Modified (Based on FontForge 20230101)

## 📋 About This Modified Version

This is a modified version of FontForge 20230101 with specific fixes for macOS 15.2 compatibility and stability improvements.

## 🔧 Modifications Made

### 1. **NULL Pointer Safety Fixes**
- Fixed critical segmentation fault in `u_strmatch()` and related functions
- Added NULL pointer checks to 6 string comparison functions in `Unicode/ustring.c`:
  - `u_strmatch()` - Unicode string case-insensitive comparison
  - `u_strcmp()` - Unicode string comparison  
  - `u_strncmp()` - Unicode string comparison with length limit
  - `u_strnmatch()` - Unicode string case-insensitive comparison with length limit
  - `uc_strcmp()` - Unicode to ASCII string comparison
  - `uc_strmatch()` - Unicode to ASCII string case-insensitive comparison

### 2. **Python Environment Fixes**
- Resolved "Core python package 'pkg_resources' not found" error
- Added setuptools package to bundled Python environment
- Fixed plugin discovery functionality

### 3. **macOS 15.2 Compatibility**
- Updated build configuration for macOS 15.2
- Fixed compatibility issues with latest Xcode and macOS SDK
- Optimized for Apple Silicon and Intel architectures

## 📜 Original Copyright and License

**Original FontForge Copyright:**
- Copyright (C) 2000-2012 by George Williams
- Copyright (C) 2012-2023 by FontForge developers

**License:** 
- FontForge is available under the GNU GPL version 3 or later
- Many parts are available under the revised BSD license
- See `LICENSE` file for complete license information

## 🔧 Modifications Copyright

**Modifications Copyright (C) 2025**
- NULL pointer safety fixes
- macOS 15.2 compatibility improvements
- Python environment fixes

These modifications are released under the same license terms as the original FontForge (GPLv3+ with BSD components).

## ⚖️ License Compliance

This modified version fully complies with FontForge's open source license:

✅ **Source code availability**: All modifications are available in source form  
✅ **License preservation**: All original license notices retained  
✅ **Attribution**: Original authors properly credited  
✅ **Modification notice**: Changes clearly identified and documented  
✅ **Same license**: Distributed under compatible license terms  

## 🚀 Installation and Usage

This modified version works exactly like the original FontForge, with the following improvements:

- **Stable startup**: No more crashes when opening file dialogs
- **Clean Python environment**: No pkg_resources warnings
- **macOS 15.2 optimized**: Full compatibility with latest macOS

## 🔗 Links

- **Original FontForge**: https://fontforge.org/
- **Original Repository**: https://github.com/fontforge/fontforge
- **Issue Reports**: Use the original FontForge issue tracker for general issues
- **License Information**: https://fontforge.org/license.html

## 📝 Disclaimer

This is an **unofficial modified version** of FontForge. While it includes important stability fixes, it is not endorsed by the original FontForge development team. For official releases, please visit the original FontForge website.

## 🤝 Contributing

If you find these modifications useful, consider contributing the fixes back to the original FontForge project at https://github.com/fontforge/fontforge

---

**Build Date**: 2025-07-20  
**Based on**: FontForge 20230101  
**Platform**: macOS 15.2 (Universal Binary) 