---
description: >-
  User Roles allow you to group sets of permissions and assign them to the users
  in your organization.
---

# Manage Roles

If you don't want to give a user full access to the Cloud Management Platform, you can let them perform only a subset of tasks by assigning a role. Roles make it easy to assign multiple permissions and manage users more efficiently in your organization. 

{% hint style="info" %}
Required permission to manage and assign roles: **User Manager**
{% endhint %}

{% hint style="warning" %}
Prior to Roles, CMP users were manually assigned permissions. These legacy permissions are forward-compatible, so you will not lose access to any functionalities you previously had access to.
{% endhint %}

### Pre-built roles

There are a few pre-built roles in your account for your convenience. The easiest way to give user privileges is to assign pre-built roles. Each role grants one or more privileges that together, allow performing a common business function. For example, one role allows managing user accounts, another role manages financial aspects, another role manages IT functions, and so on.

#### **Basic Role**

| Privileges | Only users with privilege can:  |
| :--- | :--- |
| Support | create new and access existing technical support requests  |

#### **IT Manager**

| Privileges | Only users with privilege can:  |
| :--- | :--- |
| Support | create new and access existing technical support requests |
| Manage Licenses | buy and manage Google Workspace and Office 365 Licenses |

#### **Finance User**

| Privileges | Only users with privilege can:  |
| :--- | :--- |
| Support | create new and access existing technical support requests |
| Billing Profiles Admin  | create new and manage existing billing profiles, including payment method |
| Invoice Viewer | access invoices |
| Cloud Analytics | create new and access existing Cloud Analytics Reports |

#### **Standard User**

| Privileges | Only users with privilege can:  |
| :--- | :--- |
| Support | create new and access existing technical support requests |
| Cloud Analytics  | create new and access existing Cloud Analytics Reports |
| Sandbox User | create disposable cloud environments \(sandboxes\) according to company policy |
| superQuery | unlimited access to the superQuery IDE |

#### **Power User**

| Privileges | Only users with privilege can:  |
| :--- | :--- |
| Support | create new and access existing technical support requests |
| Cloud Analytics  | create new and access existing [Cloud Analytics Reports](../cloud-analytics/create-cloud-report.md) |
| Sandbox User | [create disposable cloud environments](../cloud-sandbox-management/create-gcp-sandbox-accounts.md) \(sandboxes\) governed by a company Sandbox policy |
| superQuery | access superQuery IDE |
| Sandbox Admin | set company [Sandbox policy](../cloud-sandbox-management/configuring-a-policy-for-sandbox-accounts.md) for other users  |
| FlexRI Admin | purchase and manage [flexible reservations](../flexible-reservations/flexri.md) |
| Manage Settings | manage your Cloud Management Platform account settings |

#### **Admin**

Has access to all features in the Cloud Management Platform and the CMP API, and can manage every aspect of your organization's account. 

**Summary: Pre-built Roles and Permissions** 

<table>
  <thead>
    <tr>
      <th style="text-align:left">Permissions</th>
      <th style="text-align:center"><b>Admin</b>
      </th>
      <th style="text-align:center">
        <p><b>Finance</b>
        </p>
        <p><b>User</b>
        </p>
      </th>
      <th style="text-align:center">
        <p><b>IT</b>
        </p>
        <p><b>Manager</b>
        </p>
      </th>
      <th style="text-align:center">
        <p><b>Power</b>
        </p>
        <p><b>User</b>
        </p>
      </th>
      <th style="text-align:center">
        <p><b>Standard</b>
        </p>
        <p><b>User</b>
        </p>
      </th>
      <th style="text-align:center">
        <p><b>superQuery</b>
        </p>
        <p><b>User</b>
        </p>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Billing Profile Admin</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Cloud Analytics</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Flexible RI Admin</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&lt;em&gt;&lt;/em&gt;</td>
    </tr>
    <tr>
      <td style="text-align:left">Invoice Viewer</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&lt;em&gt;&lt;/em&gt;</td>
    </tr>
    <tr>
      <td style="text-align:left">Licenses Manager</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Manage Settings</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Sandbox Admin</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Sandbox User</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">Users Manager</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
    </tr>
    <tr>
      <td style="text-align:left">superQuery</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center"></td>
      <td style="text-align:center"></td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
      <td style="text-align:center">&#x2714;</td>
    </tr>
  </tbody>
</table>

### Custom Roles

If one of the built-in roles doesn't work for you, you can create a custom role with your own set of permissions. To create a custom user role, select the "Users and Roles" icon in the lefthand navigation bar.

![](../.gitbook/assets/usersandroles.jpg)

From there, navigate to the "Roles" tab. You will see a list of Preset Roles, as well as any other Custom Roles created by your team.

![](../.gitbook/assets/rolestab.jpg)

Create a new role by clicking on the "**+ NEW** " button at the top right of the screen. This opens a new page with a [list of permissions](user-permissions-explained.md) available to group into the new role.

To get started:

1. Give your new User Role a good name.
2. _**Optional:**_ Give the role a description to give additional context around who the role is for.
3. Select the permissions you'd like the role to contain.

![](../.gitbook/assets/createrole.jpg)

### Editing a Custom Role

{% hint style="info" %}
You can't edit built-in roles.
{% endhint %}

To modify the permissions contained in a custom role, check the box next to the role you'd like to edit, then click on the "Edit Role" icon at the top-right of your screen.

![](../.gitbook/assets/editrole.jpg)

From there, make your edits to the permissions the role contains. When finished, click on the **&lt;--** back arrow icon at the top-left to return to the main Roles page.

### Deleting a Custom Role

To delete the custom role, you will need to make sure there are no users configured with this role. You cannot delete a role until this condition is satisfied. 

Select the role you'd like to delete and click the "Remove" button. You will need to confirm your action and the role will be removed.

{% hint style="info" %}
You can't remove built-in roles.
{% endhint %}

