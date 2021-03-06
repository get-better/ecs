---
keyword: [pricing, billing, question, commonly asked questions, FAQ, account, instance, image, custom image, commercial availability of Alibaba Cloud Marketplace images, subscription Alibaba Cloud Marketplace image, Block Storage, snapshot, network, P2V Cloud Migration tool]
---

# Billing FAQ

This topic provides answers to commonly asked questions about ECS billing.

-   Account FAQ
    -   [Why am I unable to purchase pay-as-you-go instances?](#section_cva_k09_jom)
    -   [How are invoices issued for pay-as-you-go instances?](#section_17y_2sv_f6a)
-   FAQ about refunds for instance downgrades
    -   [How is the refundable amount for an instance downgrade calculated?](#refund)
    -   [Why is the actual refundable amount for an instance downgrade less than that I expected?](#section_u5j_66n_sji)
-   FAQ about instance billing
    -   Billing of subscription instances
        -   [What can I do if the billing method of an instance cannot be changed from subscription to pay-as-you-go?](#section_eqx_j6c_n19)
    -   Billing of pay-as-you-go instances
        -   [How is the billable time of a pay-as-you-go instance calculated? For example, if I create a pay-as-you-go ECS instance at 2019-12-12 01:30:00 and release it at 2019-12-12 02:00:00, is the instance billed for a period of half an hour or an hour?](#section_yly_fqs_5wh)
        -   [Will a pay-as-you-go instance still incur fees after it is stopped either manually or due to an overdue payment?](#section_3u7_7sa_56q)
        -   [What can I do if an order cannot be placed to change the billing method of an instance from pay-as-you-go to subscription?](#section_byo_s8j_sva)
        -   [How long after an order is paid does it take to change the billing method of the specified instance from pay-as-you-go to subscription?](#section_rsw_jya_q3n)
        -   [What can I do if the billing method of an instance cannot be changed from pay-as-you-go to subscription?](#section_w9t_g35_3r8)
        -   [When I change the billing method of an instance from pay-as-you-go to subscription, will the billing method for network usage of the instance also change?](#section_2be_3hw_11z)
        -   [I have an unpaid order to change the billing method of an instance from pay-as-you-go to subscription. If I upgrade the instance, will the order still be valid?](#section_x7u_ki5_5vd)
        -   [Why am I unable to change a pay-as-you-go instance to a subscription one?](#section_asw_2pt_juv)
    -   No Fees for Stopped Instances \(VPC-Connected\) feature
        -   [To which types of ECS instances is the No Fees for Stopped Instances \(VPC-Connected\) feature applicable?](#section_ufh_c2k_8kc)
        -   [Can I retain the compute and network resources of a stopped pay-as-you-go instance after I enable the No Fees for Stopped Instances \(VPC-Connected\) feature?](#section_mhp_hoi_tbr)
        -   [Can ECS instances that are stopped from within their operating systems enter the No Fees for Stopped Instances \(VPC-Connected\) state?](#section_si5_ui9_2lf)
        -   [Can ECS instances that use local disks enter the No Fees for Stopped Instances \(VPC-Connected\) state?](#section_jfw_0rx_5vk)
        -   [When I started an instance immediately after it enters the No Fees for Stopped Instances \(VPC-Connected\) state, an OperationConflict error was reported. Why?](#section_ss5_caj_eit)
        -   [When I called the StartInstance operation to start an instance in the No Fees for Stopped Instances \(VPC-Connected\) state, an OperationDenied.NoStock error was reported. Why?](#section_o8e_zoo_bkq)
        -   [I set Stop Mode of an instance to No Charges After Instance Is Stopped. The instance was stopped and entered the No Fees for Stopped Instances \(VPC-Connected\) state. When I restarted this instance, its public IP address changed. How do I prevent the IP address from changing?](#section_kd0_w0b_tmj)
    -   Instance billing
        -   [Can I release ECS instances on my own?](#section_8e6_x1p_ch4)
        -   [When I try to change the billing method of a disk in an ECS instance, an error message is returned indicating that I have already changed the billing method of the disk three times. What does this mean?](#section_uiw_o96_c0k)
        -   [Why has a pay-as-you-go bill been generated for my instance? What are the fees on the bill?](#section_yk7_8r8_8g9)
        -   [Why am I unable to change the billing method of instances from pay-as-you-go to subscription?](#section_2bu_739_jyz)
        -   [Why am I unable to change the billing method of instances from subscription to pay-as-you-go?](#section_rzg_62t_xq0)
-   FAQ about image billing
    -   Billing of public images
        -   [Do I need to pay for Red Hat images when you use them to create ECS instances?](#section_r69_pvd_25l)
        -   [How are Windows licenses billed? Are they billed based on countries and the numbers of cores?](#section_pjr_p5e_w91)
    -   Billing of custom images
        -   [How am I charged when I copy a custom image?](#section_tnl_2sp_tay)
        -   [I am creating an ECS instance. Why is the displayed total instance cost higher when I select a custom image than when I select a public image?](#section_i6r_iol_dmz)
    -   Billing of Alibaba Cloud Marketplace images
        -   [Are Alibaba Cloud Marketplace images refundable?](#section_iuv_e0g_ryy)
        -   [After Alibaba Cloud Marketplace images have become commercially available, are there still any free Alibaba Cloud Marketplace images?](#section_wjg_0ut_ph0)
        -   [When I upgrade and renew an instance created from an Alibaba Cloud Marketplace image, do I need to make further payments?](#section_z81_o2e_mwr)
        -   [After an instance created from an Alibaba Cloud Marketplace image is released, can I continue to use that image for free when I purchase a new ECS instance?](#section_atl_uoh_7ny)
        -   [I created an ECS instance from an Alibaba Cloud Marketplace image and then created a custom image from the instance. Do I need to pay for the custom image when I use it to create a new ECS instance?](#section_1rq_tsr_1kg)
        -   [If I copy a custom image derived from an Alibaba Cloud Marketplace image to another region to create an ECS instance, do I need to pay for the custom image?](#section_yg0_dk3_kt4)
        -   [If I share a custom image derived from an Alibaba Cloud Marketplace image to Account B, does Account B need to pay to use the custom image to create an ECS instance?](#section_2z1_84u_1oo)
        -   [Will I be charged if I use an Alibaba Cloud Marketplace image or a custom image derived from an Alibaba Cloud Marketplace image to replace a system disk?](#section_f17_kdh_l8i)
        -   [Will I be charged if I replace the system disk of an ECS instance that runs an Alibaba Cloud Marketplace image?](#section_ap2_oad_813)
    -   Billing of subscription Alibaba Cloud Marketplace images
        -   [What are yearly, monthly, and weekly subscription Alibaba Cloud Marketplace images?](#section_swr_l61_ikk)
        -   [In what ECS instances can subscription images be used?](#section_av8_o6w_fgc)
        -   [How do I purchase a subscription image? Can I purchase it separately?](#section_4j4_46c_bjh)
        -   [How do I pay for a subscription image?](#section_erh_8ee_ikm)
        -   [Can I use a subscription image after it expires? How do I continue to use an expired subscription image?](#section_bti_h6m_can)
        -   [Can I request a refund if I no longer need a subscription image after purchase?](#section_pfw_vyx_lg4)
        -   [How are fees settled after a refund is made?](#section_ul7_mda_7hn)
        -   [Can a subscription image be converted to a pay-as-you-go image?](#section_l8h_x3l_gxw)
        -   [Can I replace a subscription image with an image of another type or vice versa? How will I be charged for the image after the replacement?](#section_gna_w0n_odz)
        -   [Will I be charged if I use a subscription image to create a custom image? How will the created custom image be affected if the subscription image expires?](#section_qih_xuj_v4g)
-   FAQ about Block Storage billing
    -   [How is an enhanced SSD \(ESSD\) billed?](#section_2hn_vx7_4rt)
    -   [How do I purchase a standard SSD? What are the pricing options for I/O optimized instances and standard SSDs?](#section_gvg_7ni_aoz)
    -   [How is a separately purchased pay-as-you-go data disk billed?](#section_r7r_ux5_0ko)
-   FAQ about snapshot billing
    -   [The snapshots from which existing disks or custom images were created will be retained for 15 days after a payment in my account becomes overdue. Will these snapshots continue to incur fees, adding to the amount of the overdue payment?](#section_nf7_257_f6v)
-   FAQ about network usage billing
    -   [How is the public bandwidth of ECS instances billed?](#section_dwe_br6_fgi)
    -   [How are inbound traffic and outbound traffic of pay-as-you-go instances billed?](#section_zu4_9tq_fdz)
    -   [What is the difference between pay-by-bandwidth and pay-by-traffic?](#section_2xb_e9k_5kz)
    -   [Can I adjust the specified peak bandwidth?](#section_sy1_fpd_1tk)
    -   [Will traffic generated by ECS instances under attack incur fees?](#section_8m0_xjn_x7l)
    -   Pay-by-traffic billing of public bandwidth for subscription instances
        -   [Can I select the pay-by-traffic billing method for network usage when I purchase a subscription instance?](#section_833_hn8_tap)
        -   [How are you charged when you select the pay-by-traffic billing method for network usage?](#section_4vz_zc9_gnc)
        -   [Can I change the billing method for network usage of a subscription instance from pay-by-bandwidth to pay-by-traffic?](#section_re1_ou7_60i)
        -   [Can I adjust the peak bandwidth for traffic for an ECS instance at any time?](#section_ei9_f8i_d64)
        -   [When I renewed a subscription instance, I upgraded or downgraded the instance and changed its billing method for network usage from pay-by-traffic to pay-by-bandwidth. Why is the public bandwidth service of the instance still stopped after the change?](#section_fgm_ns8_60p)
        -   [If the pay-by-traffic billing method is used for a subscription instance, can the instance continue to use the public bandwidth service when a payment becomes overdue for the instance due to insufficient account balance?](#section_ekv_ozx_v9t)
        -   [If the pay-by-traffic billing method is used for a subscription instance, will I be notified when a payment becomes overdue for the instance in my account?](#section_nhh_cph_mpe)
        -   [If the pay-by-traffic billing method is used for a subscription instance, can I upgrade the instance after a payment becomes overdue for the instance in my account?](#section_wxp_s0g_s4k)
        -   [If the pay-by-traffic billing method is used for a subscription instance, is the public bandwidth service of the instance automatically resumed after I settle overdue payments?](#section_cch_foi_y6h)
        -   [How is traffic priced after I change the billing method for network usage of a subscription instance from pay-by-bandwidth to pay-by-traffic?](#section_zql_gig_uz6)

## Why am I unable to purchase pay-as-you-go instances?

You may be unable to purchase pay-as-you-go instances due to one of the following reasons:

-   You have not passed real-name verification. To purchase ECS instances within any regions in mainland China, you must pass [real-name verification](https://www.alibabacloud.com/help/doc-detail/52595.htm).
-   The number of vCPUs consumed by the selected pay-as-you-go instance type exceeds the vCPU quota for pay-as-you-go instances of your account.
-   Resources of the selected instance type are unavailable for purchase within the selected region. Try again later or go to the [ECS Instance Types Available for Each Region](https://ecs-buy.aliyun.com/instanceTypes/#/instanceTypeByRegion) page to view instance types available in each region.

## How are invoices issued for pay-as-you-go instances?

You can apply for invoices for your pay-as-you-go instances. Only one invoice is provided based on your monthly statement. Go to the [Billing Management](https://billing.console.aliyun.com/) console to apply for invoices.

## How is the refundable amount for an instance downgrade calculated?

Alibaba Cloud will determine how to calculate the refundable amount for an instance downgrade based on the payment currency specified on your order to purchase the instance.

-   If the payment currency is USD, the **price difference-based method** is used to calculate the refundable amount.
-   If the payment currency is a currency other than USD, such as Malaysian ringgit \(MYR\) or Indian rupee \(INR\), the **ratio-based method** is used.

Remaining value: Alibaba Cloud linearly allocates the value of each subscription ECS instance to the instance subscription period. The value of each subscription instance diminishes over time. The value that a subscription instance has is its remaining value. When you cancel the subscription of an instance after you have used the instance for a certain period of time, the remaining value of the instance can be refunded to you. For example, assume that you purchased an instance for a 30-day term at the price of USD 30. If you cancel the subscription of the instance after you have used it for 10 days, the remaining value of the instance of USD 20 will be refunded to you.

When you used a currency other than USD to pay for the order, the order amount was converted to the payment currency at the prevailing exchange rate at the time of payment. Therefore, that exchange rate will be considered during the calculation of the instance remaining value. As opposed to the **price difference-based method**, the **ratio-based method** ensures that refunds will be made based on the exchange rates at the time of payment. This prevents the amount refunded for instance downgrades from being affected by exchange rate fluctuations.

**Note:**

-   Instance downgrades do not change the lifecycles of instances.
-   If you have used different currencies to purchase and upgrade an instance, the instance cannot be downgraded.

The following examples demonstrate how to use the price difference-based method to calculate the refundable amounts for instance downgrades:

-   Example 1: New Instance A is downgraded after it has been in use for some period of time.

    Assume that on the first day of a calendar month, you purchased Instance A for a 30-day term at the price of USD 1/day and paid USD 30 in total. On the 11th day of the calendar month, you initiate a downgrade of the instance. The price of the new instance configurations is USD 0.5/day. The refundable amount for the instance downgrade is calculated in the following manner:

    1.  Calculate the remaining value M of Instance A.

        M = USD 30 × \(30 days -10 days\)/30 days = USD 20

    2.  Calculate the value N of the new instance configurations.

        The instance lifecycle remains unchanged before and after the downgrade. You can use the new instance configurations for only 20 days. The following formula is used to calculate N: N = USD 0.5/day × 20 days = USD 10.

    3.  Calculate the refundable amount.

        Refundable amount = M - N = USD 20 - USD 10 = USD 10

    In this example, Alibaba Cloud will refund USD 10 for the instance downgrade.

-   Example 2: New Instance B has been upgraded after it was in use for some period of time, and is downgraded after another period of time.

    Assume that on the first day of a calendar month, you purchased Instance B for a 30-day term at the price of USD 1/day and paid USD 30 in total. On the 11th day of the calendar month, you upgraded the instance. The price of the new instance configurations was USD 2/day. You paid the price difference P between the original and new instance configurations. The following formula is used to calculate P: P = \(USD 2/day - USD 1/day\) × \(30 days - 10 days\) = USD 20. On the 21th day of the calendar month, you initiate a downgrade of the instance. The price of the new instance configurations is USD 0.5/day. The refundable amount is calculated in the following manner:

    1.  Calculate the remaining value M of Instance B.

        Because the instance has been upgraded, the remaining value of the instance consists of the remaining value M1 from instance purchase and the remaining value M2 from the instance upgrade. The following formulas are used to calculate M1 and M2:

        -   M1 = USD 30 × \(30 days -20 days\)/30 days = USD 10
        -   M2 = USD 20 × \(20 days -10 days\)/20 days = USD 10
        M = M1 + M2 = USD 20

    2.  Calculate the value N of the new instance configurations.

        The instance lifecycle remains unchanged before and after the downgrade. You can use the new instance configurations for only 10 days. The following formula is used to calculate N: N = USD 0.5/day × 10 days = USD 5.

    3.  Calculate the refundable amount.

        Refundable amount = M - N = USD 20 - USD 5 = USD 15

    In this example, Alibaba Cloud will refund USD 15 for the instance downgrade.


The following examples demonstrate how to use the ratio-based method to calculate the refundable amount in MYR for instance downgrades:

-   Example 1: New Instance A is downgraded after it has been in use for some period of time.

    Assume that on the first day of a calendar month, you placed an order to purchase Instance A for a 30-day term and the order amount was USD 30. The MYR to USD exchange rate was 1:10 at the time of your purchase, and you paid MYR 300 in total. On the 11th day of the calendar month, you initiate a downgrade of the instance. The price of the new instance configurations is USD 0.5/day. The refundable amount for the instance downgrade is calculated in the following manner:

    1.  Calculate the remaining value M of Instance A.

        M = MYR 300 × \(30 days -10 days\)/30 days = MYR 200

    2.  Calculate the refund ratio R.

        R = \(USD 1/day - USD 0.5/day\)/USD 1/day = 1/2

    3.  Calculate the refundable amount.

        Refundable amount = M × R = MYR 200 × 1/2 = MYR 100

    In this example, Alibaba Cloud will refund MYR 100 for the instance downgrade.

-   Example 2: New Instance B has been upgraded after it was in use for some period of time, and is downgraded after another period of time.

    Assume that on the first day of a calendar month, you placed an order to purchase Instance B for a 30-day term and the order amount was USD 30. The MYR to USD exchange rate was 1:10 at the time of your purchase. You paid MYR 300 in total. On the 11th day of the calendar month, you upgraded the instance. The price of the new instance configurations was USD 2/day. The MYR to USD exchange rate was 1:11 at the time of upgrade. You paid the price difference P between the original and new instance configurations. The following formula is used to calculate P: P = \(USD 2/day - USD 1/day\) × \(30 days - 10 days\) × 11 = MYR 220. On the 21th day of the calendar month, you initiate a downgrade of the instance. The price of the new instance configurations is USD 0.5/day. The refundable amount is calculated in the following manner:

    1.  Calculate the remaining value M of Instance B.

        Because the instance has been upgraded, the remaining value of the instance consists of the remaining value M1 from instance purchase and the remaining value M2 from the instance upgrade. The following formulas are used to calculate M1 and M2:

        -   M1 = USD 30 × \(30 days -20 days\)/30 days × 10 = MYR 100
        -   M2 = USD 20 × \(20 days -10 days\)/20 days × 11 = MYR 110
        M = M1 + M2 = MYR 210

    2.  Calculate the refund ratio R.

        R = \(USD 2/day - USD 0.5/day\)/USD 2/day = 3/4

    3.  Calculate the refundable amount.

        Refundable amount = M × R = M1 × R + M2 × R = MYR 100 × 3/4 + MYR 110 × 3/4 = MYR 157.5

    In this example, Alibaba Cloud will refund MYR 157.5 for the instance downgrade.


## Why is the actual refundable amount for an instance downgrade less than that I expected?

If you purchased the instance at a discounted rate or if the instance price changes before the downgrade, the actual refundable amount may be less than that you expected.

For example, assume that you purchased an instance for a 30-day term at the price of USD 1/day, and that the MYR to USD exchange rate was 1:10 at the time of your purchase. You paid MYR 300 for the instance. 10 days later, you initiate a downgrade of the instance, and the price of the new instance configurations is USD 0.5/day. The refundable amount is MYR 100 as calculated based on the original instance price of USD 1/day. However, if you purchased the instance at a discounted rate or if the instance price changes before the downgrade, the actual refundable amount is calculated based on the non-discounted or new price. For example, assume that the instance price has changed to USD 0.7/day before the downgrade. The refundable amount is calculated in the following manner:

1.  Calculate the remaining value M of Instance A.

    M = MYR 300 × \(30 days -10 days\)/30 days = MYR 200

2.  Calculate the refund ratio R.

    R = \(USD 0.7/day - USD 0.5/day\)/USD 1/day = 1/5

3.  Calculate the refundable amount.

    Refundable amount = M × R = MYR 200 × 1/5 = MYR 40


In this example, the actual refundable amount is MYR 40 instead of MYR 100.

## What do I do if the billing method of an instance cannot be changed from subscription to pay-as-you-go?

You may be unable to change the billing method of an instance from subscription to pay-as-you-go due to one of the following reasons:

-   The instance is in a state that does not support changes to the billing method. For example, the instance has an unpaid order.
-   The instance is in the **Expired** state.
-   The instance information has changed. For example, the bandwidth of the instance has been temporarily upgraded.

If one of the preceding errors is reported, adjust the instance accordingly. If the problem persists, [submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex).

## How is the billable time of a pay-as-you-go instance calculated? For example, if I create a pay-as-you-go ECS instance at 2019-12-12 01:30:00 and release it at 2019-12-12 02:00:00, is the instance billed for a period of half an hour or an hour?

Pay-as-you-go instances are billed on one second increments. Payments are made at the top of each hour. The billable time of pay-as-you-go instances is automatically calculated. For example, if you create a pay-as-you-go instance at 2019-12-12 01:30:00 and release it at 2019-12-12 02:00:00, the hour from 01:00:00 to 02:00:00 is a billing cycle. The billable time is 1,800 seconds, which is calculated with the following formula: \(30 minutes\) × 60 = 1800 seconds.

## Am I still charged for a pay-as-you-go instance after it is stopped either manually or due to an overdue payment?

**Stopped due to an overdue payment**: When a payment becomes overdue in your account, your pay-as-you-go instance is automatically stopped and billing for this instance stops. Instances do not always stay in the Stopped state after they are stopped due to overdue payments. For more information, see [Pay-as-you-go](/intl.en-US/Pricing/Billing methods/Pay-as-you-go.md).

**Manually stopped**: You can stop a running pay-as-you-go instance by using the ECS console or by calling the StopInstance operation. When the instance is stopped, its status changes to **Stopped**. Billing for stopped pay-as-you-go instances is based on their network types.

-   VPC: You can enable the No Fees for Stopped Instances \(VPC-Connected\) feature.
    -   After the feature is enabled, billing for pay-as-you-go instances in VPCs starts when the instances are created, stops when the instances enter the **Stopped** state, and resumes when the instances are started. When a pay-as-you-go instance enters the Stopped state, the No Fees for Stopped Instances \(VPC-Connected\) feature stops billing only for the vCPUs, memory, and public IP address of the instance. Other resources such as disks and EIPs of the instance continue to be billed. For more information, see [No Fees for Stopped Instances \(VPC-Connected\)](/intl.en-US/Pricing/Billing methods/No Fees for Stopped Instances (VPC-Connected).md).
    -   After the feature is disabled, billing for pay-as-you-go instances continues when they are stopped.
-   Classic network: ECS instances in the classic network are billed regardless of whether they are in the **Stopped** state.

## What do I do if an order cannot be placed to change the billing method of an instance from pay-as-you-go to subscription?

You may be unable to place the order due to one of the following reasons:

-   The instance is in a state that does not support changes to the billing method. For example, the instance has an unpaid order.
-   Changes to the billing method are not allowed due to an upcoming scheduled automatic release.
-   Changes to the billing method are not allowed because the instance information has changed.
-   A previous order to change the billing method of the instance has not been paid.

If one of the preceding errors is reported, adjust the instance accordingly.

## How long after an order is paid does it take to change the billing method of an instance from pay-as-you-go to subscription?

The billing method of your ECS instance is changed after the order is paid. It can take up to four seconds to change the billing method of 20 instances. After the change is complete, you can see that the billing method of your instance has been changed to **Subscription** in the ECS console.

## What do I do if the billing method of an instance cannot be changed from pay-as-you-go to subscription?

[Submit a ticket](https://workorder-intl.console.aliyun.com/#/ticket/createIndex).

## When I change the billing method of an instance from pay-as-you-go to subscription, does the billing method for network usage of the instance also change?

No, the billing method for network usage of the instance does not change. Only the billing method of instances and disks can be changed from pay-as-you-go to subscription. For information about how to change the billing method for network usage, see [Overview of instance upgrade and downgrade](/intl.en-US/Instance/Change configurations/Overview of instance upgrade and downgrade.md).

## I have an unpaid order to change the billing method of an instance from pay-as-you-go to subscription. If I upgrade the configurations of the instance, is the order still valid?

An order is created when you change the billing method of your instance from pay-as-you-go to subscription. You must pay for the order to complete the change. If you upgrade the configurations of the instance before the order is paid, the order payment cannot be completed because the instance components are different and the original order no longer matches. If you still want to change the billing method of your instance, you must cancel the unpaid order and place a new order.

## Why am I unable to change a pay-as-you-go instance into a subscription one?

The pay-as-you-go instance that you want to change must meet the following requirements:

-   The instance type of the instance is not retired. For more information, see [Phased-out instance types](/intl.en-US/Instance/Phased-out instance types.md).
-   The instance is not a preemptible instance.
-   No unpaid orders related to the instance exist.

    If unpaid orders related to the instance exist, you must pay for the orders or cancel the orders before you change the billing method of the instance.

-   Automatic release time is not configured for the instance.

    If automatic release time is set for the instance, you must disable the automatic release configuration before you change the billing method. For more information, see [Disable automatic release](/intl.en-US/Instance/Manage instances/Release an instance.md).

-   The instance is in the **Running** or **Stopped** state.

    Example: An order to change the billing method was placed while the ECS instance is in the Running or Stopped state. However, the instance status changes before the payment was attempted. The order fails and the billing method does not change. You can go to the Billing Management console and pay for the order when the instance is in the Running or Stopped state again.


## To which types of ECS instances is the No Fees for Stopped Instances \(VPC-Connected\) feature applicable?

The No Fees for Stopped Instances \(VPC-Connected\) feature is applicable to ECS instances that meet the following requirements:

-   The network type of the instances is VPC.
-   The instances use the pay-as-you-go billing method.
-   The instances do not use local disks.

For more information, see [No Fees for Stopped Instances \(VPC-Connected\)](/intl.en-US/Pricing/Billing methods/No Fees for Stopped Instances (VPC-Connected).md).

## Can I retain the compute and network resources of a stopped pay-as-you-go instance after I enable the No Fees for Stopped Instances \(VPC-Connected\) feature?

With the No Fees for Stopped Instances \(VPC-Connected\) feature enabled, you still can configure whether a pay-as-you-go instance enters the No Fees for Stopped Instances \(VPC-Connected\) state by setting the Stop Mode parameter when you stop the instance. If the instance does not enter the No Fees for Stopped Instances \(VPC-Connected\) state after it is stopped, its compute and network resources will not be released.

If you only need to stop an instance for a few minutes before it is restarted, we recommend that you configure the instance not to enter the No Fees for Stopped Instances \(VPC-Connected\) state by performing one of the following operations: Call the [StopInstance](/intl.en-US/API Reference/Instances/StopInstance.md) operation with StoppedMode set to KeepCharging, or set Stop Mode to **Retain Instance and Continue Charging After Instance Is Stopped** when you stop the instance from the ECS console.

## Can ECS instances that are stopped from within their operating systems enter the No Fees for Stopped Instances \(VPC-Connected\) state?

No, ECS instances that are stopped from within their operating systems cannot enter the No Fees for Stopped Instances \(VPC-Connected\) state. Only ECS instances that are stopped by one of the following methods can enter the No Fees for Stopped Instances \(VPC-Connected\) state:

-   Use the ECS console.
-   Use ECS API.

## Can ECS instances that use local disks enter the No Fees for Stopped Instances \(VPC-Connected\) state?

No, ECS instances that use local disks cannot enter the No Fees for Stopped Instances \(VPC-Connected\) state.

## When I started an instance immediately after it enters the No Fees for Stopped Instances \(VPC-Connected\) state, an OperationConflict error was reported. Why?

When an instance enters the No Fees for Stopped Instances \(VPC-Connected\) state, its compute resources \(CPUs and memory\) and public IP address are recycled. If you only need to stop an instance for a few minutes before it is restarted, we recommend that you set StoppedMode to KeepCharging to disallow the instance from entering the No Fees for Stopped Instances \(VPC-Connected\) state.

## When I called the StartInstance operation to start an instance in the No Fees for Stopped Instances \(VPC-Connected\) state, an OperationDenied.NoStock error was reported. Why?

When an instance enters the No Fees for Stopped Instances \(VPC-Connected\) state, its compute resources are recycled. If instance resources are insufficient, an OperationDenied.NoStock error is reported when you attempt to start the instance. We recommend that you try again later.

## I set Stop Mode of an instance to No Charges After Instance Is Stopped. The instance was stopped and entered the No Fees for Stopped Instances \(VPC-Connected\) state. When I restarted this instance, its public IP address changed. How do I prevent the IP address from changing?

When an instance enters the No Fees for Stopped Instances \(VPC-Connected\) state, its public IP address is released. When the instance is restarted, it is assigned a new public IP address.

To retain the original public IP address of the instance, you can convert this IP address to an Elastic IP address \(EIP\) before you stop the instance. For more information, see [Convert the public IP address of a VPC-type instance to an Elastic IP address](/intl.en-US/Network/Change IPv4 addresses/Convert the public IP address of a VPC-type instance to an Elastic IP address.md) and [ConvertNatPublicIpToEip](/intl.en-US/API Reference/Networks/ConvertNatPublicIpToEip.md).

**Note:** After the IP address is converted to an EIP, you will be charged for the EIP while the instance is in the No Fees for Stopped Instances \(VPC-Connected\) state. For more information, see [Billing method](/intl.en-US/Pricing/Billing.md) of the EIP documentation.

## Can I release ECS instances on my own?

Yes, you can manually release or schedule the automatic release of pay-as-you-go instances, but you cannot release subscription instances on your own.

If you have further questions, [submit a ticket](https://workorder-intl.console.aliyun.com/console.htm).

## When I attempt to change the billing method of a disk in an ECS instance, an error message is returned indicating that I have already changed the billing method three times. What does this mean?

Each ECS instance can have its configurations downgraded a maximum of three times. Downgrade operations include downgrades of instance specifications, bandwidth downgrades, and the change of the disk billing method from subscription to pay-as-you-go.

## Why has a pay-as-you-go bill been generated for my instance? What are the fees on the bill?

You can copy your instance ID and perform the following steps to view the bill details:

1.  Log on to the [ECS console](https://ecs.console.aliyun.com).
2.  In the top navigation bar, choose **Billing** \> **User Center**.
3.  In the left-side navigation pane, choose **Spending Summary** \> **Instance Spending Detail**.
4.  Set the search criteria.

    ![](https://static-aliyun-doc.oss-accelerate.aliyuncs.com/assets/img/en-US/5291909951/p55292.png)


## Why am I unable to change the billing method of instances from pay-as-you-go to subscription?

The billing method of instances of the following instance types cannot be changed from pay-as-you-go to subscription:

-   Instance types of Generation One: t1, s1, s2, s3, m1, m2, c1, and c2
-   Instance types in the n1, n2, and e3 instance families

**Note:** For more information about the preceding instance types, see [Phased-out instance types](/intl.en-US/Instance/Phased-out instance types.md).

If your pay-as-you-go instances are not of the preceding instance types, ensure that the instances meet the requirements to change their billing method to subscription. For more information, see [Change the billing method of an instance from pay-as-you-go to subscription](/intl.en-US/Pricing/Change the billing method/Change the billing method of an instance from pay-as-you-go to subscription.md).

## Why am I unable to change the billing method of instances from subscription to pay-as-you-go?

Whether the billing method of subscription instances can be changed to pay-as-you-go depends on your ECS usage. Before you change the billing method of subscription instances, ensure that the instances are in the **Running** or **Stopped** state.

## Do I need to pay for Red Hat images when you use them to create ECS instances?

Yes, you must pay for Red Hat images when you use them to create ECS instances. Red Hat images are paid images. For pricing details, see the ECS pricing page.

## How are Windows licenses billed? Are they billed based on countries and the numbers of cores?

Windows licenses are free of charge within regions in mainland China but are charged in regions outside of mainland China. The charges for Windows licenses vary with countries, regions, and the numbers of vCPUs. For pricing details, see the ECS pricing page.

## How am I charged when I copy a custom image?

You must perform the following operations to copy a custom image:

1.  Copy the snapshot from which the custom image was created from the source region to the destination region.
2.  Create a custom image from the snapshot in the destination region.

You may be charged the following fees for the preceding operations:

-   Fees for traffic between the two regions. Alibaba Cloud does not charge you for cross-region traffic. For the latest billing details, see the official Alibaba Cloud website for announcements.
-   The new snapshot \(snapshot copy\) consumes snapshot storage space in the destination region. Snapshots are billed based on the storage space used. For more information, see [Snapshot](/intl.en-US/Pricing/Billing items/Snapshot billing.md).

## I am creating an ECS instance. Why is the total instance cost displayed when I select a custom image higher than that displayed when I select a public image?

This situation may occur in the following circumstances:

-   The custom image contains data disk snapshots. When such an image is selected, the costs of the data disks cause the total cost of the instance to be higher than that of an instance created from a public image.
-   The custom image was created based on a paid public image such as a Windows Server or RHEL image.

## Are Alibaba Cloud Marketplace images refundable?

Alibaba Cloud Marketplace images support money-back guarantee within a certain period of time based on the Alibaba Cloud Marketplace rules. However, you are ineligible for a refund in the following situations:

-   You have deployed the purchased image to an ECS instance within the money-back guarantee period.
-   You have deployed the purchased image to an ECS instance before your application for a refund for this image is approved.
-   You can receive refunds only for images that have not been used.

## Are free Alibaba Cloud Marketplace images still available after Alibaba Cloud Marketplace images are commercially available?

Free Alibaba Cloud Marketplace images are still available. However, you must purchase them at a price of USD 0.00 before you can use them.

## I have an instance created from an Alibaba Cloud Marketplace image. Do I need to make further payments for the image when I renew the instance or upgrade its configurations?

No, you do not need to make further payments for the image. After you purchase an Alibaba Cloud Marketplace image, you can use it on instances at no additional costs.

## I have an ECS instance created from an Alibaba Cloud Marketplace image. After the instance is released, can I continue to use that image free of charge when I purchase a new ECS instance?

Yes, you can continue to use that image free of charge when you purchase a new ECS instance.

## I created an ECS instance from an Alibaba Cloud Marketplace image and then created a custom image from the instance. Do I need to pay for the custom image when I use it to create an ECS instance?

Yes, you must pay the original price of the Alibaba Cloud Marketplace image.

## If I copy an Alibaba Cloud Marketplace image that I bought to another region to create an ECS instance, do I need to pay for the image?

Yes, you must pay the original price of the Alibaba Cloud Marketplace image.

## I created an ECS instance from an Alibaba Cloud Marketplace image and then created a custom image from that instance. If I share the custom image to Account B, does Account B need to pay for the custom image when it uses this image to create an ECS instance?

Yes, Account B must pay the original price of the Alibaba Cloud Marketplace image.

## Is a fee charged if I replace a system disk by using an Alibaba Cloud Marketplace image or an image derived from an Alibaba Cloud Marketplace image?

It depends. If the current image of your ECS instance is a different version of the replacement image, no fees are charged. Otherwise, a fee is charged.

## My ECS instance is using an Alibaba Cloud Marketplace image. Is a fee charged if I replace the system disk of the instance?

No, no fees are charged if you replace the system disk of the instance.

## What are yearly, monthly, and weekly subscription Alibaba Cloud Marketplace images?

Yearly, monthly, or weekly subscription Alibaba Cloud Marketplace images are images that are purchased from Alibaba Cloud Marketplace and billed on a subscription basis. These images are developed and maintained by image providers, who are responsible for both pre-sales consultation and after-sales services. In this topic, these images are collectively referred to as subscription images.

## On which ECS instances can I use a subscription image?

A subscription image can only be used on a subscription instance with the same subscription duration.

## How do I purchase a subscription image? Can I purchase it separately?

No, you cannot purchase a subscription image separately.

You can use one of the following methods to purchase a subscription image:

-   When you create an ECS instance, set Billing Method to **Subscription**, select an **Alibaba Cloud Marketplace** image, and then specify a subscription duration by setting Duration.

    **Note:** In this case, you must pay for both the instance and the image. The instance is created on successful payment for both the image and instance.

-   To use a subscription image on an existing subscription ECS instance, you can use the image to replace the operating system of the instance. In this case, you must select the image subscription duration based on the instance subscription duration. For more information, see [Replace a system disk \(non-public images\)](/intl.en-US/Block Storage/Cloud disks/Change the operating system/Replace a system disk (non-public images).md).

    **Note:** In this case, you only need to pay for the image.


## How do I pay for subscription images?

Subscription images require payment upfront. The subscription duration of a subscription image must be the same as that of the subscription instance on which the image is used.

Image prices are set by the image providers.

## Can I use a subscription image after it expires? How do I continue to use it?

When a subscription image expires, it cannot be used unless it is renewed in a timely manner.

You cannot renew a subscription image separately. If you want to continue using the image, you must renew the image together with the corresponding ECS instance. You can resume use of the image after it is renewed.

## After I purchase a subscription image, can I request a refund if I no longer want to use it?

The image provider determines whether to make a refund. You can consult the image provider before you purchase the image.

## What can I expect when a refund is made?

If a refund is available, the image provider makes the refund based on your usage.

## Can a subscription image be converted to a pay-as-you-go image?

Subscription images cannot be converted to pay-as-you-go images. This conversion function is currently under development for release in the future. Stay updated on the official Alibaba Cloud website.

## Can I replace a subscription image with an image of another type or vice versa? How is the fee calculated?

Yes, you can replace images when you replace system disks of ECS instances. You can make the following replacements:

-   Replace an image of another type \(such as public image, custom image, or shared image\) with a subscription image. After the image is replaced, the system calculates the actual cost based on the image cost and the remaining subscription duration of the ECS instance.
-   Replace a subscription image with an image of another type \(such as public image, custom image, or shared image\). If the image provider allows for refunds, a refund is made based on your actual usage.
-   Replace Subscription Image A with Subscription Image B. If a refund is available after the image is replaced, the refund is made based on the refund policy. The actual cost of Image B is calculated based on the image price and the remaining subscription duration of the ECS instance.

## Is a fee charged for a custom image derived from a subscription image? How is the custom image affected if the subscription image expires?

When you use a custom image derived from a subscription image to create an instance or replace a system disk, you are re-ordering the subscription image on Alibaba Cloud Marketplace. The custom image is not affected regardless of whether the subscription image expires.

## How are enhanced SSDs billed?

Enhanced SSDs support both subscription and pay-as-you-go billing methods. For more information, see the [Pricing](https://www.alibabacloud.com/product/ecs) page.

## How do I purchase a standard SSD? What are the pricing options for I/O optimized instances and standard SSDs?

For pricing details, see the [Pricing](https://www.alibabacloud.com/product/ecs) page.

## How is a separately purchased pay-as-you-go data disk billed?

A pay-as-you-go data disk is billed by the hour. Note that if your account balance is insufficient, the services of the data disk will be suspended.

## The snapshots from which existing disks or custom images were created will be retained for 15 days after a payment in my account becomes overdue. Will these snapshots continue to incur fees, adding to the amount of the overdue payment?

No, the snapshots will not continue to incur fees.

For example, your account has an overdue payment of USD 0.1. After the 15-day retention period, the snapshots from which no existing disks or custom images were created will be deleted. The snapshots from which existing disks or custom images were created will be retained and will not incur additional charges. To use these retained snapshots, you must settle the overdue payment first but you do not have to pay for them again.

## How is the network usage of ECS instances billed?

For information about how the network usage of ECS instances is billed, see [Public bandwidth](/intl.en-US/Pricing/Billing items/Public bandwidth.md).

## How are inbound traffic and outbound traffic of pay-as-you-go instances billed?

Traffic between ECS instances or between ECS instances and other Alibaba Cloud services within the same local area network \(LAN\) is free of charge. Traffic between ECS instances and the Internet is billed based on the following rules:

-   Inbound Internet traffic is free of charge. Inbound Internet traffic refers to the traffic from the Internet to ECS instances, such as traffic that is generated when you download resources from the Internet to your ECS instances or when your users upload resources to your ECS instances by using the FTP client.
-   Outbound Internet traffic is billed. Outbound Internet traffic refers to the traffic from ECS instances to the Internet, such as the traffic that is generated when your ECS instances provide external access or when your users download internal resources from your ECS instances by using the FTP client.

For more information about bandwidth billing, see [Public bandwidth](/intl.en-US/Pricing/Billing items/Public bandwidth.md).

## What is the difference between pay-by-bandwidth and pay-by-traffic?

If you select pay-by-bandwidth as the billing method for network usage, you are charged based on the specified bandwidth. Your actual outbound bandwidth will not exceed the specified bandwidth.

If you select pay-by-traffic as the billing method for network usage, you are charged based on the actual volume of traffic. To prevent unmanageable fees incurred from traffic bursts, you can set a peak bandwidth for outbound Internet traffic.

For more information, see [Public bandwidth](/intl.en-US/Pricing/Billing items/Public bandwidth.md).

## Can I adjust the specified peak bandwidth?

Yes, you can adjust the specified peak bandwidth. For more information, see [Overview of instance upgrade and downgrade](/intl.en-US/Instance/Change configurations/Overview of instance upgrade and downgrade.md).

## Will traffic generated by ECS instances under attack incur fees?

The inbound Internet traffic generated by ECS instances under attack will not incur fees, but the outbound Internet traffic will.

We recommend that you use Alibaba Cloud Security services such as Server Guard to reinforce the security of your ECS instances.

## Can I select the pay-by-traffic billing method for network usage when I purchase a subscription instance?

Yes, you can select the pay-by-traffic billing method for network usage when you purchase a subscription instance. For more information, see [Create an instance by using the wizard](/intl.en-US/Instance/Create an instance/Create an instance by using the wizard.md).

For more information about pay-by-traffic billing method, see the [Elastic Compute Service](https://www.alibabacloud.com/product/ecs) page.

## How are you charged when you select the pay-by-traffic billing method for network usage?

Pay-by-traffic is a pay-as-you-go billing method in which fees are charged based on the volume of traffic consumed. Payments are settled at the top of each hour. To keep services running properly, ensure that your account balance is sufficient. To prevent unmanageable fees incurred from traffic bursts, you can set a peak bandwidth for traffic.

## Can I change the billing method for network usage of a subscription instance from pay-by-bandwidth to pay-by-traffic?

Yes, you can change the billing method for network usage of a subscription instance from pay-by-bandwidth to pay-by-traffic by using the bandwidth downgrade feature. However, you can make this change a limited number of times. For more information, see [Modify the bandwidth configurations of subscription instances](/intl.en-US/Instance/Change configurations/Modify bandwidth configurations/Modify the bandwidth configurations of subscription instances.md).

You can also use the renewal and upgrade or downgrade feature to change the billing method for network usage. The new configurations do not take effect until the next subscription period starts. For more information, see [Downgrade the configurations of an instance during renewal](/intl.en-US/Pricing/Renew instances/Downgrade the configurations of an instance during renewal.md).

## Can I adjust the peak bandwidth for traffic for an ECS instance at any time?

Yes, you can adjust the peak bandwidth for traffic for an ECS instance by using the bandwidth downgrade feature at any time. After you set the peak bandwidth to a smaller value, the new value takes effect immediately. A maximum of three refunds can be made for each instance. Exercise caution when you downgrade an instance.

If you upgraded or downgraded a subscription instance when it was renewed, you cannot upgrade or downgrade the instance again until the new subscription period starts.

## When I renewed a subscription instance, I upgraded or downgraded the instance and changed its billing method for network usage from pay-by-traffic to pay-by-bandwidth. Why is the public bandwidth service of the instance still stopped after the change?

If you upgrade or downgrade a subscription instance and change its billing method for network usage when you renew the instance, the new configurations will not take effect until the new subscription period starts. Although you paid for the new subscription period, if payments become overdue for the instance before the new subscription period starts, the pay-by-traffic public bandwidth service of the instance will be stopped.

If payments remain overdue, the public bandwidth service will remain stopped even after the new subscription period starts. To keep the service running properly, ensure that your account balance is sufficient.

## If the pay-by-traffic billing method is used for a subscription instance, can the instance continue to use the public bandwidth service when a payment becomes overdue for the instance due to insufficient account balance?

Overdue payments do not affect the running of subscription instances, but do cause the pay-by-traffic public bandwidth service to be stopped, preventing the instances from accessing the Internet. You can continue to use the public bandwidth service only after you settle the overdue payment. To keep the service running properly, ensure that your account balance is sufficient.

## If the pay-by-traffic billing method is used for a subscription instance, will I be notified when a payment becomes overdue for the instance in my account?

Yes, you will be notified by SMS. To keep services running properly, ensure that your account balance is sufficient.

## If the pay-by-traffic billing method is used for a subscription instance, can I upgrade the instance after a payment becomes overdue for the instance in my account?

No, you can upgrade the instance only after you settle the overdue payment.

## If the pay-by-traffic billing method is used for a subscription instance, is the public bandwidth service of the instance automatically resumed after I settle overdue payments?

If the public bandwidth service was stopped due to an overdue payment, the service will automatically resume when the overdue payment is settled.

## How is traffic priced after I change the billing method for network usage of a subscription instance from pay-by-bandwidth to pay-by-traffic?

When you change the billing method for network usage of your subscription instance from pay-by-bandwidth to pay-by-traffic, you are billed for network usage based on the actual volume of traffic. Payments are settled at the top of each hour. For pricing details, see the [Elastic Compute Service](https://www.alibabacloud.com/zh/product/ecs#pricing) page.

