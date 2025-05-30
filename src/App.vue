<template>
	<div class="my-5 glacvcd-sr-form-wrap">
		<form
			ref="form"
			enctype="multipart/form-data"
			:id="form_id"
			class="kwes-form"
			action="https://kwes.io/api/foreign/forms/zy3GwS7cnN2JHQzK90z1"
			multistep
			no-reload
		>
			<div class="kw-multistep">
				<G-Step heading="Intro">
					<b-alert variant="danger" show>
						COVID-19 Note Layla Serrano: Please be advised the District performs
						property inspections on a case-by-case basis and will be
						conducted contact-free with the resident.
						<a
							href="https://www.glacvcd.org/our-response-to-covid-19"
							><strong>Read More >></strong></a
						>
					</b-alert>
					<hr />
					<h2>
						Submitting a Service Request? Here’s what to expect.
					</h2>
					<div style="margin:15px 0;max-width:560px;">
						<div
							class="embed-responsive embed-responsive-16by9"
							style="height:auto;"
						>
							<iframe
								src="https://www.youtube.com/embed/bOQ_cyGos50"
								allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
								allowfullscreen=""
								width="760"
								height="515"
								frameborder="0"
								class="embed-responsive-item"
							></iframe>
						</div>
					</div>
					<p>
						<span style="font-size: 16px;"
							>When calling regarding mosquito bites on a
							residential property, an inspector will be
							dispatched to inspect the caller's property first to
							identify potential breading sources. The inspector
							will provide guidance regarding long-term control
							and source reduction, and will also address other
							potential sources in the immediate vicinity.</span
						>
					</p>
					<h3>Mosquito Control is a Shared Responsibility</h3>
					<h4>What We Control</h4>
					<p>
						Greater Los Angeles County Vector Control
						District<strong><em> only </em></strong>provides
						services for:
					</p>
					<ol style="font-weight:bold;">
						<li>Mosquitoes</li>
						<li>Midges</li>
						<li>Black Flies</li>
					</ol>
					<p>
						Our public healthy agency provides services for 35
						cities and parts of unincorporated Los Angeles County
						free of charge.
					</p>
					<h4>How are Requests Handled?</h4>
					<p>
						Submitted service requests are handled on a case-by-case
						basis. When mosquito bites are reported on an immediate
						property, an inspector will be dispatched to the
						caller's property first to clear the property before
						inspecting the vicinity. Mosquitoes do not fly far and
						cryptic breeding sources are often found nearby.
					</p>
					<p>
						The service request entry you submit may result in an
						investigation or action on someone else’s private
						property. Personal information is required but will
						remain confidential and will not be made public or
						shared with any other party as permitted by law. The
						District may contact you for further information but
						will not provide further updates or details regarding
						the case.
					</p>
					<h4>What to do While You Wait</h4>
					<p>
						<b
							>Eliminate any standing water in and outside your
							property.</b
						><br />Mosquitoes grow in dirty, standing water. Our
						District routinely checks public spaces throughout our
						service area but we need your help in removing any
						standing water from your property. For a list of common
						sources and solutions, visit our
						<strong
							><a
								href="https://www.glacvcd.org/do-it-yourself-solutions-for-mosquito-problems"
								>Do-It-Yourself Mosquito Solutions Resource
								Page.&nbsp;</a
							></strong
						>
					</p>
					<p>
						<b>Wear insect repellent.</b><br />If adult mosquitoes
						are active, wear insect repellent to prevent mosquito
						bites and mosquito-transmitted diseases.
						<strong
							><a
								href="https://www.glacvcd.org/repellent-information"
								>Learn which ingredients are recommended by the
								Centers for Disease Control and
								Prevention.&nbsp;</a
							></strong
						>
					</p>
					<p>
						<b>Share with Your Community.<br /></b>Stay up-to-date
						on the best ways to get rid of mosquitoes and disease
						activity in your area, and share with your community.
						Follow us on social media or&nbsp;sign up for our
						<a
							href="https://www.glacvcd.org/subscribe-to-our-mailing-list"
							><strong>E-Alerts</strong></a
						>.
					</p>

					<hr class="x-hr" />

					<h2 class="h-custom-headline h3">
						<span>Ready to Submit a Service Request?</span>
					</h2>

					<b-alert variant="danger" show>
						COVID-19 Note:&nbsp;&nbsp;Please be advised the District
						performs property inspections on a case-by-case basis
						and will be conducted contact-free with the resident.
						<a
							href="https://www.glacvcd.org/our-response-to-covid-19"
							><strong>Read More &gt;&gt;</strong></a
						>
					</b-alert>

					<p>Click "Next" to continue submitting your request.</p>

					<p>
						<strong>Confidential reporting:&nbsp;</strong>The
						information you provide will be used for the sole
						purpose of directing resources in the fight against
						mosquito-borne diseases. Personal information will
						remain confidential and will not be made public or
						shared with any other party as permitted by law.
					</p>
				</G-Step>
				<G-Step heading="Service Request Type">
					<!--<b-form-group
						data-kw-group
						rules="not_regex:/^(Bees|Rodents)/"
					>-->
					<b-form-group data-kw-group rules="required">
						<b-form-radio-group
							id="service-request-type"
							name="WaterSource"
							v-model="form.WaterSource"
							@change="scrollToNext"
							stacked
						>
							<div class="row">
								<div class="col">
									<span class="h2 d-block text-center"
										>Service Request Type</span
									>
								</div>
							</div>
							<div
								class="row row-cols-2 row-cols-md-3 row-cols-xl-4 align-content-stretch"
							>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Mosquitoes"
										src="images/mosquitoes.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Black Flies"
										src="images/black-flies.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Midges"
										src="images/midges.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Mosquitofish Request"
										src="images/mosquitofish.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Standing Water"
										src="images/standing-water.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Neglected Pool"
										src="images/neglected-pool.jpg"
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Other"
										src="images/other.jpg"
									></image-radio-button>
								</div>
							</div>
							<div class="row mt-4">
								<div class="col-12">
									<span class="h2 d-block text-center"
										>Pests We Don't Service</span
									>
								</div>
							</div>
							<div
								class="row row-cols-2 row-cols-md-3 row-cols-xl-4 align-content-stretch"
							>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Bees"
										src="images/bees.jpg"
										invalid
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Rodents"
										src="images/rodents.jpg"
										invalid
									></image-radio-button>
								</div>
								<div class="col mt-4 d-flex flex-column">
									<image-radio-button
										value="Fire Ants"
										src="images/ants.png"
										invalid
									></image-radio-button>
								</div>
							</div>
							<g-alert
								v-show="form.WaterSource == 'Mosquitoes'"
								class="mt-4"
							>
								<div class="row">
									<div class="col-12 col-md-4 col-xl-2">
										<img
											style="width:120px;"
											class="mr-2"
											src="./assets/images/mosquito-quarter.jpg"
										/>
									</div>
									<div class="col">
										<p>
											Adult mosquitoes are about a quarter
											inch big. If your pest is bigger,
											you're probably dealing with a
											different vector.
											<a
												href="https://www.glacvcd.org/mosquitoes"
												>Check out this page</a
											>
											for help identifying your pest.
										</p>
									</div>
								</div>
							</g-alert>
							<g-alert
								v-show="form.WaterSource == 'Black Flies'"
								class="mt-4"
							>
								<div class="row">
									<div class="col-12 col-md-4 col-xl-2">
										<img
											style="width:120px;"
											class="mr-2"
											src="./assets/images/black-flies.jpg"
										/>
									</div>
									<div class="col">
										<p>
											Black flies are common within 1 mile
											of the LA River.
											<a
												href="https://www.glacvcd.org/other-vectors-and-insects"
												target="_blank"
												>Please visit our black flies
												guide</a
											>
											to verify you have black flies
											before submitting this request.
										</p>
									</div>
								</div>
							</g-alert>
							<g-alert
								v-show="form.WaterSource == 'Standing Water'"
								class="mt-4"
							>
								<div class="row">
									<div class="col">
										<p>
											Standing water on your own property
											can often be self-mitigated. Check
											out
											<a
												href="https://www.glacvcd.org/do-it-yourself-solutions-for-mosquito-problems"
												>these resources for preventing,
												removing, or treating standing
												water on your property</a
											>
											before submitting a service request.
										</p>
									</div>
								</div>
							</g-alert>
							<g-alert
								v-show="form.WaterSource == 'Bees'"
								class="mt-4"
								variant="danger"
							>
								<div class="row align-items-center">
									<div class="col">
										<p class="mb-0">
											GLACVCD does not respond to bees.
											You should contact a private pest
											control company, or the
											<a
												href="https://acwm.lacounty.gov/bees-in-our-environment/"
												target="_blank"
												>LA County Agricultural
												Commissioner of Weights and
												Measures</a
											>
											at (626) 575-5471 or their Bee
											Hotline at 1-800-BEE-WARY
											(1-800-233-9279)
										</p>
									</div>
								</div>
							</g-alert>
							<g-alert
								v-show="form.WaterSource == 'Rodents'"
								class="mt-4"
								variant="danger"
							>
								<div class="row align-items-center">
									<div class="col">
										<p class="mb-0">
											GLACVCD does not respond to rodents.
											Instead, contact the
											<a
												href="http://www.publichealth.lacounty.gov/eh/SSE/Vector_Management/vmvcontrol.htm"
												>LA County Department of Health
												Services, Vector Management
												Program</a
											>
											at (626) 430-5461
										</p>
									</div>
								</div>
							</g-alert>
							<g-alert
								v-show="form.WaterSource == 'Fire Ants'"
								class="mt-4"
								variant="danger"
							>
								<div class="row align-items-center">
									<div class="col">
										<p class="mb-0">
											GLACVCD does not respond to
											cockroaches, fire ants, or
											run-of-the-mill houseflies. You
											should contact private pest control.
										</p>
									</div>
								</div>
							</g-alert>
						</b-form-radio-group>
					</b-form-group>
					<input-group
						ref="bites_occurring"
						label="When are mosquito bites occurring?"
					>
						<b-form-checkbox-group
							name="BiteTimes"
							v-model="form.BiteTimes"
							rules="min:1"
							class="required"
							required
							:options="when_are_bites_occurring_options"
							stacked
						></b-form-checkbox-group>
					</input-group>
					<input-group label="Additional details about the situation">
						<b-form-textarea
							name="Comments"
							class="required"
							v-model="form.Comments"
							required
						></b-form-textarea>
					</input-group>
				</G-Step>
				<G-Step heading="Contact Information">
					<input-group label="Case Number">
						<b-form-input
							name="CaseNumber"
							v-model="form.CaseNumber"
							rules="max:50"
						></b-form-input>
						<b-form-text>If you've been assigned one</b-form-text>
					</input-group>
					<input-group label="Name">
						<b-form-input
							name="Name"
							rules="required|max:100"
							v-model="form.Name"
						></b-form-input>
					</input-group>
					<input-group label="Email">
						<b-form-input
							name="Email"
							v-model="form.Email"
							type="email"
							rules="max:200"
						></b-form-input>
					</input-group>
					<input-group label="Phone">
						<b-form-input
							name="Phone"
							rules="required|max:100"
							v-model="form.Phone"
							type="tel"
						></b-form-input>
					</input-group>
					<input-group label="How did you hear about us?">
						<b-form-checkbox-group
							name="RefferalSource"
							v-model="form.RefferalSource"
							:options="how_did_you_hear_options"
							stacked
							style="column-count:2"
						></b-form-checkbox-group>
					</input-group>
					<input-group
						label="How did you hear about us (other)?"
						v-show="form.RefferalSource.includes('Other')"
					>
						<b-form-input
							name="RefferalSourceOther"
							v-model="form.RefferalSourceOther"
							rules="max:500"
						></b-form-input>
					</input-group>
				</G-Step>
				<G-Step heading="Location Information">
					<input-group label="Address to report">
						<address-verifier
							ref="address_verifier"
							v-model="form.AddressObject"
						></address-verifier>
					</input-group>
					<input-group label="Additional building info">
						<b-form-input
							name="BuildingInfo"
							v-model="form.BuildingInfo"
							rules="max:100"
						></b-form-input>
						<b-form-text
							>Building, apartment, or suite number,
							etc.</b-form-text
						>
					</input-group>
					<input-group label="Property Access Information ">
						<b-form-input
							name="GateCodes"
							v-model="form.GateCodes"
							rules="max:2000"
						></b-form-input>
						<b-form-text>Gate codes, entry codes, etc.</b-form-text>
					</input-group>
					<input-group label="Nearest cross street">
						<b-form-input
							name="NearestCrossSt"
							v-model="form.NearestCrossSt"
							rules="max:500"
						></b-form-input>
					</input-group>
					<input-group label="Do you live at this address?">
						<b-form-radio-group
							name="YourAddress"
							v-model="form.YourAddress"
							required
							:options="[
								{ text: 'Yes', value: true },
								{ text: 'No', value: false },
							]"
							stacked
						></b-form-radio-group>
					</input-group>
					<input-group label="Do you have chickens in your yard?">
						<b-form-radio-group
							name="Chickens"
							v-model="form.Chickens"
							required
							:options="[
								{ text: 'Yes', value: true },
								{ text: 'No', value: false },
							]"
							stacked
						></b-form-radio-group>
					</input-group>
				</G-Step>
				<G-Step heading="Images">
					<input-group label="Upload helpful images (optional)">
						<b-form-file
							name="Image1"
							@change="handleImage($event, 'image1')"
							placeholder="Select file"
							rules="image|max:4000"
						></b-form-file>
						<b-form-file
							name="Image2"
							@change="handleImage($event, 'image2')"
							placeholder="Select file"
							rules="image|max:4000"
							class="mt-2"
						></b-form-file>
						<b-form-text>Limit 2 images, 4MB each</b-form-text>
					</input-group>
				</G-Step>
				<G-Step heading="Review & Submit">
					<p>
						Greater Los Angeles County Vector Control Technicians
						conduct site inspections on weekdays between 7am & 3pm
						during the regular mosquito season. Best efforts will be
						made to accommodate the property owner's availability
						but it is not guaranteed during the season. Inspections
						may be conducted when resident/owner is not present only
						with pre-authorization and scheduled appointment.
					</p>
					<p>
						Your privacy matters to us. The District considers all
						reports and requests for service confidential, and will
						not disclose the requests unless California law requires
						such disclosure. Your information will not be sold or
						shared with other parties.
					</p>
				</G-Step>
			</div>
		</form>
	</div>
</template>

<script>
import GStep from "./components/Kwes/GStep.vue";
import GAlert from "./components/GAlert.vue";
import InputGroup from "./components/Form/InputGroup.vue";
import ImageRadioButton from "./components/Form/ImageRadioButton.vue";
import kwesforms from "kwesforms";
import AddressVerifier from "./components/Form/AddressVerifier.vue";
import axios from "axios";
import {
	BFormGroup,
	BAlert,
	BFormText,
	BFormRadioGroup,
	BFormInput,
	BFormFile,
	BFormCheckboxGroup,
	BFormTextarea,
} from "bootstrap-vue";
import { pick, isEmpty } from "lodash";

export default {
	name: "App",
	components: {
		GAlert,
		GStep,
		ImageRadioButton,
		InputGroup,
		AddressVerifier,
		BFormGroup,
		BAlert,
		BFormText,
		BFormRadioGroup,
		BFormInput,
		BFormFile,
		BFormCheckboxGroup,
		BFormTextarea,
	},
	data() {
		return {
			form_id: "glacvcd-form",
			form: {
				WaterSource: "",
				BiteTimes: [],
				Comments: "",
				CaseNumber: "",
				Name: "",
				Email: "",
				Phone: "",
				RefferalSource: [],
				BuildingInfo: "",
				GateCodes: "",
				NearestCrossSt: "",
				YourAddress: null,
				Chickens: null,
				image1: null,
				image2: null,
				AddressObject: {},
			},
			when_are_bites_occurring_options: [
				"Night",
				"Day/Afternoon",
				"Not getting bites",
			],
			how_did_you_hear_options: [
				"From prior experience",
				"Word of mouth",
				"Google search",
				"Heard/read in news",
				"Nextdoor",
				"Social media",
				"Community event",
				"Advertisement",
				"Other",
			],
			endpoint: "https://sr.glacvcdops.com/Api/DeveloperSRS",
		};
	},
	mounted() {
		var vm = this;
		kwesforms.init({
			onReady() {
				kwesforms.setCustomRule(
					vm.form_id,
					"map_status",
					'The address you entered is not in our service area. Please visit <a style="text-decoration:underline;" href="https://www.glacvcd.org/links-to-agencies-to-help-with-vectors">this resource page</a> to find your local vector control district.',
					value => {
						return value == "outside";
					}
				);
				kwesforms.setCustomRule(
					vm.form_id,
					"map_status",
					"The address you entered is not specific enough. Please enter a complete address.",
					value => {
						return value == "vague";
					}
				);
				kwesforms.setCustomRule(
					vm.form_id,
					"map_status",
					"Address required. Please use the auto-complete to locate the address.",
					value => {
						return value == "";
					}
				);
				kwesforms.setCustomRule(
					vm.form_id,
					"map_status",
					"There's a problem with the address you've entered. Please use the auto-complete feature to select an address.",
					value => {
						return !["vague", "outside", "valid"].includes(value);
					}
				);
				kwesforms.setCustomRule(
					vm.form_id,
					"WaterSource",
					"Your selection is not a valid service request.",
					value => {
						console.log(value);
						return ["Bees", "Rodents", "Fire Ants"].includes(value);
					}
				);
			},
		});

		this.$refs.form.addEventListener("kwMultistepNextSuccess", () => {
			this.$refs.address_verifier.refresh();
		});

		this.$refs.form.addEventListener("kwMultistepPrevSuccess", () => {
			this.$refs.address_verifier.refresh();
		});

		this.$refs.form.addEventListener("kwSubmitted", () => {
			// e.preventDefault();
			this.submit();
		});
	},

	computed: {
		formFormatted() {
			let formatted = pick(this.form, [
				"WaterSource",
				"BiteTimes",
				"Comments",
				"CaseNumber",
				"Name",
				"Email",
				"Phone",
				"RefferalSource",
				"BuildingInfo",
				"GateCodes",
				"NearestCrossSt",
				"YourAddress",
				"Chickens",
			]);

			if (!isEmpty(this.form.AddressObject)) {
				let street_address_parts = [];

				for (
					let index = 0;
					index < this.form.AddressObject.address_components.length;
					index++
				) {
					const element =
						this.form.AddressObject.address_components[index];
					if (element["types"].includes("street_number")) {
						street_address_parts[0] = element["short_name"];
					} else if (element["types"].includes("route")) {
						street_address_parts[1] = element["short_name"];
					} else if (element["types"].includes("locality")) {
						formatted.City = element["short_name"];
					} else if (element["types"].includes("postal_code")) {
						formatted.ZipCode = element["short_name"];
					}
				}

				formatted.Address = street_address_parts.join(" ");
				if (!formatted.ZipCode) formatted.ZipCode = "00000";
				formatted.lat = this.form.AddressObject.geometry.location.lat();
				formatted.lng = this.form.AddressObject.geometry.location.lng();
			}

			formatted.BiteTimes = formatted.BiteTimes.join(",");
			formatted.RefferalSource = formatted.RefferalSource.join(",");

			return formatted;
		},
	},

	methods: {
		async submit() {
			let data = this.formFormatted;
			let base64Images = [];

			let images = [this.form.Image1, this.form.Image2];
			for (let index = 0; index < images; index++) {
				if (images[index] != null) {
					base64Images.push(images[index]);
				}
			}

			data.Images = base64Images.join(",");

			axios.post(this.endpoint, data, {}).then(
				() => {
					window.location.href =
						"https://glacvcd.org/thank-you-for-submitting-a-service-request";
				},
				error => {
					const options = {
						value1: JSON.stringify(error),
					};

					axios
						.post(
							"https://maker.ifttt.com/trigger/glacvcd_error/with/key/tD8Zx_Y3NghBPLvw-Hlv367xD1eKhDfXfLa6G0Z0XC",
							JSON.stringify(options)
						)
						.then(() => {
							//
						})
						.catch(error => {
							console.log(error);
						});

					alert(
						"Your submission failed for an unknown reason. Please contact GLACVCD at 562-944-9656 to ensure service."
					);
				}
			);
		},

		handleImage(e, field) {
			const image = e.target.files[0];
			this.storeBase64Image(image, field);
		},

		storeBase64Image(image, field) {
			var _ = this;
			const reader = new FileReader();
			reader.onload = e => {
				_.form[field] = e.target.result;
			};

			reader.readAsDataURL(image);
		},

		scrollToNext() {
			this.$refs.bites_occurring.$el.scrollIntoView();
		},
	},
};
</script>

<style scoped lang="scss">
.glacvcd-sr-form-wrap::v-deep {
	@import "assets/scss/variables";
	@import "node_modules/bootstrap/scss/functions";
	@import "node_modules/bootstrap/scss/variables";
	@import "node_modules/bootstrap/scss/mixins";
	@import "node_modules/bootstrap/scss/root";
	@import "node_modules/bootstrap/scss/reboot";
	@import "node_modules/bootstrap/scss/type";
	@import "node_modules/bootstrap/scss/images";
	@import "node_modules/bootstrap/scss/code";
	@import "node_modules/bootstrap/scss/grid";
	// @import "node_modules/bootstrap/scss/tables";
	@import "node_modules/bootstrap/scss/forms";
	@import "node_modules/bootstrap/scss/buttons";
	@import "node_modules/bootstrap/scss/transitions";
	// @import "node_modules/bootstrap/scss/dropdown";
	// @import "node_modules/bootstrap/scss/button-group";
	@import "node_modules/bootstrap/scss/input-group";
	@import "node_modules/bootstrap/scss/custom-forms";
	// @import "node_modules/bootstrap/scss/nav";
	// @import "node_modules/bootstrap/scss/navbar";
	// @import "node_modules/bootstrap/scss/card";
	// @import "node_modules/bootstrap/scss/breadcrumb";
	// @import "node_modules/bootstrap/scss/pagination";
	// @import "node_modules/bootstrap/scss/badge";
	// @import "node_modules/bootstrap/scss/jumbotron";
	@import "node_modules/bootstrap/scss/alert";
	// @import "node_modules/bootstrap/scss/progress";
	@import "node_modules/bootstrap/scss/media";
	// @import "node_modules/bootstrap/scss/list-group";
	// @import "node_modules/bootstrap/scss/close";
	// @import "node_modules/bootstrap/scss/toasts";
	// @import "node_modules/bootstrap/scss/modal";
	// @import "node_modules/bootstrap/scss/tooltip";
	// @import "node_modules/bootstrap/scss/popover";
	// @import "node_modules/bootstrap/scss/carousel";
	// @import "node_modules/bootstrap/scss/spinners";
	@import "node_modules/bootstrap/scss/utilities";
	@import "node_modules/bootstrap/scss/print";
	@import "node_modules/bootstrap-vue/src/index.scss";

	img {
		max-width: 100%;
	}

	.kw-color-error {
		outline: 1px solid #ff3852;
	}

	.alert-transparent {
		@include alert-variant(
			transparent,
			theme-color("primary"),
			$body-color
		);
	}

	.kw-multistep-button {
		@extend .btn;
		&.kw-multistep-button-submit,
		&.kw-multistep-button-next {
			@extend .btn-primary;
		}
	}

	fieldset + .kw-field-error-message {
		@include make-col-ready();
		@include make-col(12);
		padding-left: 2px;
		@include media-breakpoint-up(sm) {
			@include make-col(6);
			@include make-col-offset(6);
		}
		@include media-breakpoint-up(xl) {
			@include make-col(9);
			@include make-col-offset(3);
		}
	}
}
</style>
