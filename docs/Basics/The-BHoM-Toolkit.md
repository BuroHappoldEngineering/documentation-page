◀️ Previous read: _[The Adapter Actions](/Adapter-Actions)_

▶️ Next read: _[The CRUD methods](/The-CRUD-methods)_

___________________________________________________________________

<br/>

> ## ⚠️ Note ⚠️
> Before reading this page, please check out:
> - [Getting started for developers](/Getting-started-for-developers)
> - [Introduction to BHoM_Adapter](/Introduction-to-the-BHoM_Adapter)
> - [Adapter Actions](/Adapter-Actions)


<br/>

This page explains how to develop what we call a **Toolkit**.

<br/>

___________________________________________________________________

<br/>


## Contents

<!-- Start Document Outline -->

* [What is a Toolkit?](#what-is-a-toolkit)
* [Create a new software Toolkit using the BHoM Toolkit Template](#create-a-new-software-toolkit-using-the-bhom-toolkit-template)
	* [Installing the BHoM Toolkit Template](#installing-the-bhom-toolkit-template)
	* [Create the Toolkit using the Template](#create-the-toolkit-using-the-template)


<!-- End Document Outline -->

<br/>

___________________________________________________________________

<br/>

## What is a Toolkit?

A Toolkit is a Visual Studio solution that can contain one or more of the following:
- A [BHoM_Adapter](/Introduction-to-the-BHoM_Adapter) project, that allows to implement the connection with an external software.
- A [BHoM_Engine](/BH.Engine-%E2%80%90-Create-New-Algorithms) project, that should contain the Engine methods specific to your Toolkit.
- A [BHoM_oM](/BH.oM-%E2%80%90-Define-New-Objects) project, that should contain any oM class (types) specific to your Toolkit.

In order to implement a new Toolkit, we prepared a Toolkit Template that does all the scaffolding for you: [create an new Toolkit using the BHoM Toolkit Template](/BH.Adapter-%E2%80%90-Linking-to-Commercial-Software/_edit#create-a-new-software-toolkit-using-the-bhom-toolkit-template).

Once you have created the Visual Studio solution using the template, you only need to [implement the Adapter](/BH.Adapter-%E2%80%90-Linking-to-Commercial-Software/_edit#implement-the-adapter), and any Engine method and/or oM class that the Adapter should be using.

Let's get started!

## Create a new software Toolkit using the BHoM Toolkit Template

### Create a new Toolkit repository
Use the [template repository](https://github.com/BHoM/template-repository) to create a new repository. See the readme there.

## Implement the oM

The oM should contain property-only classes that make the schema for your Toolkit. All functionality should be placed in the Engine.
Functionality that is specific to a class should be defined in the Engine as an extension method. 

See /BH.oM-%E2%80%90-Define-New-Objects and /BH.Engine-%E2%80%90-Create-New-Algorithms for more information.


## Implement the Engine

The Engine should contain the functions applicable to the objects you've defined in the oM.

See /BH.Engine-%E2%80%90-Create-New-Algorithms for more information.

## Implement the Adapter

See the dedicated page to [Implementing an Adapter](/Implement-an-Adapter).