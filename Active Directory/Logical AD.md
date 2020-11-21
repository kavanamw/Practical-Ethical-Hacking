Logical AD

    The AD Schema 

        Defines every type of object that can be stored in the directory 

        Enforces rules regarding object creating and config 

        The rulebook 

    Domains  

        Boundry for applying policies to groups of objects  

        Used to group things together in an organization  

        A way to limit the scope of access to resources  

    Trees 

        Group of domains in a hierarchy of domains  

        Shares a contiguous namespace with the parent domain  

        Can have child domains  

        By default create a two way transitive trust with other domains  

    Forrest  

        A collection of one or more domain trees 

        Shares a common schema 

        Common config 

        Common global catalog to enable searching  

        Enable trusts between all domains in  the forest  

        Share the enterprise admins and schema admins groups 

    Ous  

        Organizational units 

        Containers for users, groups, computers, and other OUs 

        Rep organization hierarchically and logically  

    Trusts 

        Provides a mechanism for users to gain access to resources in another domain  

        Direction – flows from trusted domain to trusted domain, bidirectional 

        Transitive – trust relationship is extended beyond a two domain trust to include other trusted domains  

    Objects  

![GetImage.png](../../_resources/8d177c1641e2458eab0a768e51399872.png)

