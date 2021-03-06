---
title: 'Tutorial: Azure Active Directory integration with Aha! | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and Aha!.
services: active-directory
documentationCenter: na
author: jeevansd
manager: mtillman
ms.reviewer: barbkess

ms.assetid: ad955d3d-896a-41bb-800d-68e8cb5ff48d
ms.service: active-directory
ms.subservice: saas-app-tutorial
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: tutorial
ms.date: 08/09/2019
ms.author: jeedes

ms.collection: M365-identity-device-management
---

# Tutorial: Integrate Aha! with Azure Active Directory

In this tutorial, you'll learn how to integrate Aha! with Azure Active Directory (Azure AD). When you integrate Aha! with Azure AD, you can:

* Control in Azure AD who has access to Aha!.
* Enable your users to be automatically signed-in to Aha! with their Azure AD accounts.
* Manage your accounts in one central location - the Azure portal.

To learn more about SaaS app integration with Azure AD, see [What is application access and single sign-on with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-appssoaccess-whatis).

## Prerequisites

To get started, you need the following items:

* An Azure AD subscription. If you don't have a subscription, you can get a [free account](https://azure.microsoft.com/free/).
* Aha! single sign-on (SSO) enabled subscription.

## Scenario description

In this tutorial, you configure and test Azure AD SSO in a test environment.

* Aha! supports **SP** initiated SSO
* Aha! supports **Just In Time** user provisioning

## Adding Aha! from the gallery

To configure the integration of Aha! into Azure AD, you need to add Aha! from the gallery to your list of managed SaaS apps.

1. Sign in to the [Azure portal](https://portal.azure.com) using either a work or school account, or a personal Microsoft account.
1. On the left navigation pane, select the **Azure Active Directory** service.
1. Navigate to **Enterprise Applications** and then select **All Applications**.
1. To add new application, select **New application**.
1. In the **Add from the gallery** section, type **Aha!** in the search box.
1. Select **Aha!** from results panel and then add the app. Wait a few seconds while the app is added to your tenant.

## Configure and test Azure AD single sign-on for Aha!

Configure and test Azure AD SSO with Aha! using a test user called **B.Simon**. For SSO to work, you need to establish a link relationship between an Azure AD user and the related user in Aha!.

To configure and test Azure AD SSO with Aha!, complete the following building blocks:

1. **[Configure Azure AD SSO](#configure-azure-ad-sso)** - to enable your users to use this feature.
	1. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with B.Simon.
	1. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable B.Simon to use Azure AD single sign-on.
2. **[Configure Aha! SSO](#configure-aha-sso)** - to configure the Single Sign-On settings on application side.
	1. **[Create Aha! test user](#create-aha-test-user)** - to have a counterpart of B.Simon in Aha! that is linked to the Azure AD representation of user.
3. **[Test SSO](#test-sso)** - to verify whether the configuration works.

## Configure Azure AD SSO

Follow these steps to enable Azure AD SSO in the Azure portal.

1. In the [Azure portal](https://portal.azure.com/), on the **Aha!** application integration page, find the **Manage** section and select **Single sign-on**.
1. On the **Select a Single sign-on method** page, select **SAML**.
1. On the **Set up Single Sign-On with SAML** page, click the edit/pen icon for **Basic SAML Configuration** to edit the settings.

   ![Edit Basic SAML Configuration](common/edit-urls.png)

1. On the **Basic SAML Configuration** section, perform the following steps:

    a. In the **Sign on URL** text box, type a URL using the following pattern:
    `https://<companyname>.aha.io/session/new`

    b. In the **Identifier (Entity ID)** text box, type a URL using the following pattern:
    `https://<companyname>.aha.io`

	> [!NOTE]
	> These values are not real. Update these values with the actual Sign on URL and Identifier. Contact [Aha! Client support team](https://www.aha.io/company/contact) to get these values. You can also refer to the patterns shown in the **Basic SAML Configuration** section in the Azure portal.

4. On the **Set up Single Sign-On with SAML** page, in the **SAML Signing Certificate** section,  find **Federation Metadata XML** and select **Download** to download the certificate and save it on your computer.

	![The Certificate download link](common/metadataxml.png)

6. On the **Set up Aha!** section, copy the appropriate URL(s) based on your requirement.

	![Copy configuration URLs](common/copy-configuration-urls.png)

### Create an Azure AD test user

In this section, you'll create a test user in the Azure portal called B.Simon.

1. From the left pane in the Azure portal, select **Azure Active Directory**, select **Users**, and then select **All users**.
1. Select **New user** at the top of the screen.
1. In the **User** properties, follow these steps:
	1. In the **Name** field, enter `B.Simon`.  
	1. In the **User name** field, enter the username@companydomain.extension. For example, `B.Simon@contoso.com`.
	1. Select the **Show password** check box, and then write down the value that's displayed in the **Password** box.
	1. Click **Create**.

### Assign the Azure AD test user

In this section, you'll enable B.Simon to use Azure single sign-on by granting access to Aha!.

1. In the Azure portal, select **Enterprise Applications**, and then select **All applications**.
1. In the applications list, select **Aha!**.
1. In the app's overview page, find the **Manage** section and select **Users and groups**.

   	![The "Users and groups" link](common/users-groups-blade.png)

1. Select **Add user**, then select **Users and groups** in the **Add Assignment** dialog.

	![The Add User link](common/add-assign-user.png)

1. In the **Users and groups** dialog, select **B.Simon** from the Users list, then click the **Select** button at the bottom of the screen.
1. If you're expecting any role value in the SAML assertion, in the **Select Role** dialog, select the appropriate role for the user from the list and then click the **Select** button at the bottom of the screen.
1. In the **Add Assignment** dialog, click the **Assign** button.

## Configure Aha! SSO

1. To automate the configuration within Aha!, you need to install **My Apps Secure Sign-in browser extension** by clicking **Install the extension**.

	![My apps extension](common/install-myappssecure-extension.png)

2. After adding extension to the browser, click on **Setup Aha!** will direct you to the Aha! application. From there, provide the admin credentials to sign into Aha!. The browser extension will automatically configure the application for you and automate steps 3-8.

	![Setup configuration](common/setup-sso.png)

3. If you want to setup Aha! manually, open a new web browser window and sign into your Aha! company site as an administrator and perform the following steps:

4. In the menu on the top, click **Settings**.

	![Settings](./media/aha-tutorial/IC798950.png "Settings")

5. Click **Account**.
  
	![Profile](./media/aha-tutorial/IC798951.png "Profile")

6. Click **Security and single sign-on**.

	![Security and single sign-on](./media/aha-tutorial/IC798952.png "Security and single sign-on")

7. In **Single Sign-On** section, as **Identity Provider**, select **SAML2.0**.

	![Security and single sign-on](./media/aha-tutorial/IC798953.png "Security and single sign-on")

8. On the **Single Sign-On** configuration page, perform the following steps:

	![Single Sign-On](./media/aha-tutorial/IC798954.png "Single Sign-On")

	a. In the **Name** textbox, type a name for your configuration.

	b. For **Configure using**, select **Metadata File**.

    c. To upload your downloaded metadata file, click **Browse**.

    d. Click **Update**.

### Create Aha! test user

In this section, a user called B.Simon is created in Aha!. Aha! supports just-in-time user provisioning, which is enabled by default. There is no action item for you in this section. If a user doesn't already exist in Aha!, a new one is created after authentication.

## Test SSO 

In this section, you test your Azure AD single sign-on configuration using the Access Panel.

When you click the Aha! tile in the Access Panel, you should be automatically signed in to the Aha! for which you set up SSO. For more information about the Access Panel, see [Introduction to the Access Panel](https://docs.microsoft.com/azure/active-directory/active-directory-saas-access-panel-introduction).

## Additional Resources

- [ List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory ](https://docs.microsoft.com/azure/active-directory/active-directory-saas-tutorial-list)

- [What is application access and single sign-on with Azure Active Directory? ](https://docs.microsoft.com/azure/active-directory/active-directory-appssoaccess-whatis)

- [What is conditional access in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)

