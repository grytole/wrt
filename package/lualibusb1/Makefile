include $(TOPDIR)/rules.mk

PKG_NAME:=lualibusb1
PKG_VERSION:=1.0.1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/grytole/$(PKG_NAME).git
PKG_SOURCE_VERSION:=8221cd0b2465c4857118754c20203a3a90a45119
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz

include $(INCLUDE_DIR)/package.mk

define Package/lualibusb1
  SUBMENU:=Lua
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Lua libusb binding
  MAINTAINER:=Oleksandr Grytsenko <grytole@gmail.com>
  DEPENDS:=+liblua +libusb-1.0
endef

define Package/lualibusb1/description
  This is the Lua binding for the libusb-1.0 library.
endef

define Package/lualibusb1/install
	$(INSTALL_DIR) $(1)/usr/lib/lua
	$(INSTALL_BIN) $(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)/libusb1.so $(1)/usr/lib/lua/libusb1.so
endef

$(eval $(call BuildPackage,lualibusb1))
