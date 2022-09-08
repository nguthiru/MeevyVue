<template>
    <skeleton-vue>
        <section id="terms-section">
            <p><strong>Last revised on 08/09/2022</strong></p>

            <h3>Acceptance of terms of use agreements</h3>

            <p>By creating a Meevy account regardless of the device used, you agree to be bound by i) Terms of Use ii)
                privacy policy, community guidelines each of which is incorporated in this agreement, and any terms
                disclosed and agreed to by you if you purchase additional features, products, services we offer on the
                service. If you do not accept and agree to be bound by all of the terms of this agreement, please do not
                use the service.</p>
            <p>We make changes to this agreement from time to time to abide by law requirements, new features, or other
                changes. You will be updated on changes to the terms of service</p>

            <h3>Eligibility</h3>

            <p>You are not authorized to create an account unless all the following are true:</p>
            <ol>
                <li>You are at least 18 years of age</li>
                <li>You can form a binding contract with meevy</li>
                <li>You are not barred from using the service by any legal means</li>
                <li>You will comply with this agreement and all applicable laws</li>
                <li>You have never been convicted of a felony or indictable offense</li>
            </ol>

            <h3>Account </h3>

            <p>You are responsible for maintaining the confidentiality of your login credentials, which you use to sign
                up for Meevy and you are solely responsible for all activities that occur under those credentials. If
                you think someone has gained access to your account, contact us</p>

            <h3>Termination of Service</h3>
            <p>Your account may be terminated at any time without notice we believe you have violated the agreement. You
                are not entitled to refunds upon such terminations</p>
            <h3>Safety</h3>

            <p>Meevy is not responsible for the conduct of any member on or off the service. You agree to use caution in
                interaction with other members. You are solely responsible for your interactions with other members. You
                understand that Meevy does not conduct any kind of background check on its members or otherwise inquire
                into the background of its members</p>
            <h3>Rights Meevy Grants You.</h3>
            <p>Meevy grants you a personal, worldwide, royalty-free, non-assignable, nonexclusive, revocable, and
                non-sublicensable license to access and use the Service. This license is for the sole purpose of letting
                you use and enjoy the Service&rsquo;s benefits as intended by Meevy and permitted by this Agreement.
                This license and any authorization to access the Service are automatically revoked if you do any of the
                following:</p>
            <ul>
                <li>use the Service or any content contained in the Service for any commercial purposes without our
                    written consent.</li>
                <li>copy, modify, transmit, create any derivative works from, make use of, or reproduce in any way any
                    copyrighted material, images, trademarks, trade names, service marks, or other intellectual
                    property, content, or proprietary information accessible through the Service without Meevy&rsquo;s
                    prior written consent.</li>
                <li>express or imply that any statements you make are endorsed by Meevy.</li>
                <li>use any robot, bot, spider, crawler, scraper, site search/retrieval application, proxy, or other
                    manual or automatic device, method, or process to access, retrieve, index, "data mine", or in any
                    way reproduce or circumvent the navigational structure or presentation of the Service or its
                    contents.</li>
                <li>use the Service in any way that could interfere with, disrupt or negatively affect the Service or
                    the servers or networks connected to the Service.</li>
                <li>upload viruses or other malicious code or otherwise compromise the security of the Service.</li>
                <li>forge headers or otherwise manipulate identifiers to disguise the origin of any information
                    transmitted to or through the Service.</li>
                <li>"frame" or "mirror" any part of the Service without Meevy&rsquo;s prior written authorization.</li>
                <li>use meta tags or code or other devices containing any reference to Meevy or the Service (or any
                    trademark, trade name, service mark, logo, or slogan of Meevy) to direct any person to any other
                    website for any purpose.</li>
                <li>modify, adapt, sublicense, translate, sell, reverse engineer, decipher, decompile or otherwise
                    disassemble any portion of the Service, or cause others to do so.</li>
                <li>use or develop any third-party applications that interact with the Service or other members' Content
                    or information without our written consent.</li>
                <li>use, access, or publish the Meevy application programming interface without our written consent.
                </li>
                <li>probe, scan or test the vulnerability of our Service or any system or network.</li>
                <li>encourage or promote any activity that violates this Agreement.</li>
            </ul>
            <p>&nbsp;</p>

            <p>Meevy may investigate and take any available legal action in response to illegal or unauthorized uses of
                the Service, including termination of your account.</p>
            <p>Any software that we provide you may automatically download and install upgrades, updates, or other new
                features. You may be able to adjust these automatic downloads through your device's settings.</p>

        </section>
    </skeleton-vue>
</template>

<script>
import SkeletonVue from '../components/Skeleton.vue';
export default {
    name: "Terms",
    components: {
        SkeletonVue
    }
}
</script>

<style scoped>
section {
    min-height: 100vh;
    padding: 2em 0;
    font-size: smaller;
    line-height: 3;
    margin-top: 2em;
    color: rgb(27, 27, 27);
}

li {
    list-style: lower-alpha;
}
ol,ul{
    margin-left: 3em;
}
h3{
    text-transform: uppercase;
}
</style>