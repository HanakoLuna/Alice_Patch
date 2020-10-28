include $(TOPDIR)/rules.mk

PKG_NAME:=Alice_Patch
PROJECT_NAME:=Alice_Patch
PKG_VERSION:=v1.3
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	SECTION:=luci
	CATEGORY:=LuCI
	SUBMENU:=3. Applications
	TITLE:=Alice patch
endef

define Build/Compile
endef

define Package/$(PKG_NAME)/install
	$(INSTALL_DIR) $(1)/usr/share/rpcd/acl.d $(1)/usr/lib/lua/luci/i18n/ $(1)/etc/config/
	$(INSTALL_DATA) ./root/usr/share/rpcd/acl.d/luci-app-AdGuardHome.json $(1)/usr/share/rpcd/acl.d/luci-app-AdGuardHome.json
	$(INSTALL_DATA) ./root/usr/share/rpcd/acl.d/luci-app-unblockmusic.json $(1)/usr/share/rpcd/acl.d/luci-app-unblockmusic.json
	$(INSTALL_DATA) ./root/usr/share/rpcd/acl.d/luci-app-v2ray_server.json $(1)/usr/share/rpcd/acl.d/luci-app-v2ray_server.json
	$(INSTALL_DATA) ./root/usr/share/rpcd/acl.d/luci-app-vlmcsd.json $(1)/usr/share/rpcd/acl.d/luci-app-vlmcsd.json
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/chinadns.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/chinadns.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/dns-forwarder.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/dns-forwarder.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/jd-dailybonus.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/jd-dailybonus.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/openclash.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/openclash.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/ssr-plus.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/ssr-plus.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/wrtbwmon.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/wrtbwmon.zh-tw.lmo
	$(INSTALL_DATA) ./root/usr/lib/lua/luci/i18n/AdGuardHome.zh-tw.lmo $(1)/usr/lib/lua/luci/i18n/AdGuardHome.zh-tw.lmo
	$(INSTALL_DATA) ./root/etc/config/network $(1)/etc/config/network
endef

$(eval $(call BuildPackage,$(PKG_NAME)))