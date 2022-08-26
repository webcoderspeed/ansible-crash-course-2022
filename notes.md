# Ansible

> Ansible is an open-source IT engine that automates application deployment, cloud provisioning, intra service orchestration, and other IT tools.

> Ansible is easy to deploy because it does not use any agents or custom security infrastructure on the client-side, and by pushing modules to the clients. These modules are executed locally on the client-side, and the output is pushed back to the Ansible server.

> It can easily connect to clients using SSH-Keys, simplifying though the whole process. Client details, such as hostnames or IP addresses and SSH ports, are stored in the files, which are called inventory files. If you created an inventory file and populated it, then Ansible can use it.

> Ansible uses the playbook to describe automation jobs, and playbook, which uses simple language, i.e., YAML. YAML is a human-readable data serialization language & commonly used for configuration files, but it can be used in many applications where data is being stored.

> Ansible pushes small programs after connecting to your nodes which are known as "Ansible Modules". Ansible runs that module on your nodes and removes them when finished. Ansible manages the inventory in simple text files (These are the host's files). Ansible uses the host file where one can group the hosts and can control the actions on a specific group in the playbooks.

# Why Use Ansible

> Ansible is free to use by everyone.

> It is very secure due to its agentless capabilities and open SSH security features.

> Ansible does not need any special system administrator skills to install and use it.

> Ansible has a smooth learning curve determined by the comprehensive documentation and easy to learn structure and configuration.

> Its modularity regarding plugins, inventories, modules, and playbooks make Ansible perfect companion orchestrate large environments.

# Ansible History

> Michael DeHaan developed Ansible, and the Ansible project began in February 2012.

> The creator of Cobbler and Func is also the controller of the Fedora Unified network.

> RedHat acquired the Ansible tool in 2015.

> Ansible is included as part of the Fedora distribution of the Linux.

> Ansible is also available for RedHat Enterprise Linux, Debian, CentOS, Oracle Linux, and Scientific Linux via Extra Packages for Enterprise Linux (EPEL) and Ubuntu as well as for other operating systems.

# **Prerequisite**

> Hands-on experience with running commands into a Linux shell

---

# Ansible Workflow

> Ansible works by connecting to your nodes and pushing out a small program called Ansible modules to them. Then Ansible executed these modules and removed them after finished. The library of modules can reside on any machine, and there are no daemons, servers, or databases required.

<center>
<img src="./assests/ansible-works.png" alt="ansible workflow" style="background:white;padding:1rem;margin:2rem 0;"/>
</center>

> In the above image, the Management Node is the controlling node that controls the entire execution of the playbook. The inventory file provides the list of hosts where the Ansible modules need to be run. The Management Node makes an SSH connection and executes the small modules on the host's machine and install the software.

> Ansible removes the modules once those are installed so expertly. It connects to the host machine executes the instructions, and if it is successfully installed, then remove that code in which one was copied on the host machine.

## Terms used in Ansible

<table border="2">
  <thead style="background:white; color:black; font-size: 1.2rem;border: 2px solid">
    <tr>
      <th style="border-right: 2px solid">Terms</th>
      <th>Explanation</th>
    </tr>
  </thead>
  <tbody style="background:aqua; color:black; ">
    <tr>
      <td style="border: 2px solid">Ansible Server</td>
      <td style="border: 2px solid">
        It is a machine where Ansible is installed and from which all tasks and
        playbooks will be executed.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Modules</td>
      <td style="border: 2px solid">
        The module is a command or set of similar commands which is executed on
        the client-side.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Task</td>
      <td style="border: 2px solid">
        A task is a section which consists of a single procedure to be
        completed.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Role</td>
      <td style="border: 2px solid">
        It is a way of organizing tasks and related files to be later called in
        a playbook.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Fact</td>
      <td style="border: 2px solid">
        The information fetched from the client system from the global variables
        with the gather facts operation.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Inventory</td>
      <td style="border: 2px solid">A file containing the data regarding the Ansible client-server.</td>
    </tr>
    <tr>
      <td style="border: 2px solid">Play</td>
      <td style="border: 2px solid">
        It is the execution of the playbook. In simple word, a play is
        combination of multiple tasks.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Handler</td>
      <td style="border: 2px solid">The task is called only if a notifier is present.</td>
    </tr>
    <tr>
      <td style="border: 2px solid">Notifier</td>
      <td style="border: 2px solid">
        The section attributed to a task which calls a handler if the output is
        changed.
      </td>
    </tr>
    <tr>
      <td style="border: 2px solid">Tag</td>
      <td style="border: 2px solid">
        It is a name set to a task that can be used later on to issue just that
        specific task or group of jobs.
      </td>
    </tr>

  </tbody>
</table>


